---
title: Overview
---

The **ClearML Web UI** is the graphical user interface for the ClearML platform, which includes:
* Experiment management
* Browsing
* Resource utilization monitoring
* Profile management
* Direct access to the ClearML community (Slack Channel, YouTube, and GitHub).

![WebApp screenshots gif](../img/gif/webapp_screenshots.gif)

## UI Modules 
The WebApp's sidebar provides access to the following modules:
<ul>
  <li>
    <img src="/docs/latest/icons/ico-homepage.svg" alt="Homepage" className="icon size-md space-sm" /> <a href="webapp_home">Dashboard</a> - The dashboard for recent activity and quick access to experiments and projects.
  </li>
  <li> 
    <img src="/docs/latest/icons/ico-projects.svg" alt="Projects" className="icon size-md space-sm" />  <a href="webapp_projects_page">Projects</a> - The main experimentation page. Access your experiments and models as they are organized into projects.
  The <a href="webapp_exp_table">experiments</a> and <a href="webapp_model_table">models</a> are displayed in tables
  which let you:
    <ul>
      <li><a href="webapp_exp_track_visual">Track ongoing experiments and visualize their results</a></li>
      <li><a href="webapp_exp_reproducing">Reproduce previously run experiments</a></li>
      <li><a href="webapp_exp_tuning">Tune experiments with no code change</a></li>
      <li><a href="webapp_exp_comparing">Compare experiments</a></li>
      <li><a href="webapp_exp_sharing">Share experiments and their models</a> with other ClearML hosted service users </li>
    </ul>
  </li>
  <li>
    <img src="/docs/latest/icons/ico-side-bar-datasets.svg" alt="Datasets" className="icon size-md space-sm" /> <a href="datasets/webapp_dataset_page">Datasets</a> - View and manage your datasets. 
  </li>
  <li>
    <img src="/docs/latest/icons/ico-pipelines.svg" alt="Pipelines" className="icon size-md space-sm" /> <a href="pipelines/webapp_pipeline_page">Pipelines</a> - View and manage your pipelines.
  </li>
  <li>
    <img src="/docs/latest/icons/ico-reports.svg" alt="Reports" className="icon size-md space-sm" /> <a href="webapp_reports">Reports</a> - View and manage your reports.
  </li>
  <li>
    <img src="/docs/latest/icons/ico-workers.svg" alt="Workers and Queues" className="icon size-md space-sm" /> <a href="webapp_workers_queues">Orchestration</a> - Autoscale, monitor, and manage your resource usage and workers queues.
  </li>
  <li>
    <img src="/docs/latest/icons/ico-applications.svg" alt="ClearML Apps" className="icon size-md space-sm" /> <a href="applications/apps_overview">Applications</a> - ClearML's GUI applications for no-code workflow execution.
  </li>
</ul>

## UI Top Bar 
### Settings Menu

Click the profile menu button <img src="/docs/latest/icons/ico-me.svg" alt="Profile button" className="icon size-lg space-sm" />
in the top right corner of the web UI screen to access the following:
* **Settings** - Navigate to ClearML's user [Settings](webapp_profile.md) page:
  * Set WebApp preferences
  * Manage workspace API credentials
  * Configure cloud storage access credentials for the ClearML Web UI
  * ClearML Hosted service specific options
    * View usage information
    * Manage users and workspaces
    * Manage resource access permissions (available in the ClearML Enterprise plan)
* **Invite a User** to your workspace (supported in hosted service). Click **Invite a User** > input user's 
email > click **ADD** > page redirects to the [Users & Groups](webapp_profile.md#users--groups) section of 
  the **Settings** page 
* **Switch to Workspace** - Hosted service users can be members of multiple workspaces. These workspaces are listed here. 
  Click a workspace to switch to.
* **Logout** of ClearML 

### Finding What You're Looking for
Use the search bar <img src="/docs/latest/icons/ico-search.svg" alt="Magnifying glass" className="icon size-md space-sm" />
to find your ClearML resources.

To search using regex, click the `.*` icon on the search bar. 

Search results are returned for the different ClearML objects:
* Experiments - Searching an experiment table looks for matches in the experiments' name, ID, description and input and 
output models. The enterprise version also includes experiment Dataviews' hyper-datasets and versions. 
* Models - Searching a Model table looks for matches in the models' name, ID and description.
* Dataviews (Enterprise only) - Searching a Dataviews table looks for matches in the Dataviews' name, ID, description, 
hyper-datasets, and versions.
* Datasets - Searching the datasets page looks for matches in the datasets' name, ID, and description. In a dataset's
version table, a search looks for matches in the versions' name, ID, and description. 
* Pipelines - Searching the pipelines page looks for matches in the datasets' name, ID, and description. In a pipeline
run's table, a search looks for matches in the runs' name and ID. 
* Reports - Searching the reports page looks for matches in the reports' name, ID, tags, project, description, and 
report content.

The search bar in the [Dashboard](webapp_home.md) page searches the whole WebApp for objects that match queries as 
specified above and returns results divided by object type (projects, experiments, models, etc.). 

:::tip Additional filtering
ClearML's object tables (e.g. [experiments](webapp_exp_table.md), [models](webapp_model_table.md), [pipelines](pipelines/webapp_pipeline_table.md), 
and [datasets](datasets/webapp_dataset_page.md)) provide column filters to easily focus your search by object properties
(e.g status, creation/update time, metric values, etc.).
:::

### Helpful Resources 
Click the help menu button <img src="/docs/latest/icons/ico-help-outlined.svg" alt="Help menu" className="icon size-md space-sm" /> 
in the top right corner of the web UI screen to access the self-help resources including:
* ClearML Python Package setup - Instruction to get started with the `clearml` Python package
* [ClearML on YouTube](https://www.youtube.com/c/ClearML/featured) <img src="/docs/latest/icons/ico-youtube.svg" alt="Youtube" className="icon size-md space-sm" />  - Instructional videos on integrating ClearML into your workflow
* Online Documentation
* Pro Tips - Tips for working with ClearML efficiently
* [Contact Us](https://clear.ml/contact-us) - Quick access to ClearML contact form
