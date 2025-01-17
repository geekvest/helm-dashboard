# Shutting down the app
To close Helm-dashboard, click on the button in the rightmost corner of the screen. Once you click on it, your Helm-dashboard will be shut down.

![Shutdown_screenshot](images/screenshot_shut_down.png)

# Multicluster
If you want to switch to a different cluster, simply click on the corresponding cluster as shown in the figure. [Click here](https://kubernetes.io/docs/tasks/access-application-cluster/configure-access-multiple-clusters/) to learn how to access multiple clusters.
![Multicluster_screenshot](images/screenshot_multicluster.png)

# Reset Cache
The "Reset Cache" feature in Helm Dashboard clears the cached data and fetches the latest information from the backend or data source. It ensures that the dashboard displays up-to-date data and reflects any recent changes or updates.
![Detail1](images/screenshot_reset_cache.png)

# Repository
Essentially, a repository is a location where charts are gathered and can be shared. If you want to learn more about repositories, [click here](https://helm.sh/docs/topics/chart_repository/). You can find the repository in the home section, as depicted in the figure.
![Repository3](images/screenshot_repository3.png)

You can add the repository by clicking on 'Add Repository', as shown in the figure.
![Repository](images/screenshot_repository.png)

After completing that step, enter the following data: the repository name and its URL. You can also add the username and password, although this is optional.
![Repository2](images/screenshot_repository2.png)

Updating means refreshing your repository. You can update your repository as shown in the figure.
![Repository4](images/screenshot_repository4.png)

If you want to remove your repository from the Helm dashboard, click on the 'Remove' button as shown in the figure.
![Repository5](images/screenshot_repository5.png)

Use the filter option to find the desired chart quicker from the list of charts.
![Repository6](images/screenshot_repository6.png)

If you want to install a particular chart, simply hover the pointer over the chart name and an 'Install' button will appear, as shown in the figure.
![Repository7](images/screenshot_repository7.png)

# Installed Releases list
A release is an instance of your selected chart running on your Kubernetes Cluster. That means every time that you install a Helm chart there, it creates a new release or instance that coexists with other releases without conflict. You can filter releases based on namespaces or search for release names 
![Releases](images/screenshot_release.png)

The squares represent k8s resources installed by the release. Hover over each square to view a tooltip with details. Yellow indicates "pending," green signifies a healthy state, and red indicates an unhealthy state.
![Releases1](images/screenshot_release1.png)

It indicates the version of chart that corresponds to this release.
![Releases2](images/screenshot_release2.png)

A revision is linked to a release to track the number of updates/changes that release encounters.
![Releases3](images/screenshot_release3.png)
 
Namespaces are a way to organize clusters into virtual sub-clusters — they can be helpful when different teams or projects share a Kubernetes cluster. Any number of namespaces are supported within a cluster, each logically separated from others but with the ability to communicate with each other.
![Releases4](images/screenshot_release4.png)

Updated" refers to the amount of time that has passed since the last revision of the release. Whenever you install or upgrade the release, a new revision is created. You can think of it as the "age" of the latest revision.
![Releases5](images/screenshot_release5.png)

Indication of upgrade possible/repo suggested.
![Release6](images/screenshot_upgrade_available.png)

# Release details
This indicates the status of the deployed release, and 'Age' represents the amount of time that has passed since the creation of the revision until now.
![Detail](images/screenshot_release_detail.png)

You can use the Upgrade/Downgrade button to switch to different release versions, as shown in the figure.
![Detail1](images/screenshot_upgrade_available2.png)

Confirm the upgrade settings and configuration and click on confirm button to continue
![Detail2](images/screenshot_upgrade_confirmation.png)

Once the upgrade is done, your release will show the status 
![Detail3](images/screenshot_upgrade_complete.png)

It executes the test scripts or commands within the deployed application's environment and displays the results
![Detail4](images/screenshot_run_tests.png)

Running test hooks results 
![Detail5](images/screenshot_test_results.png)

The Helm Dashboard provides basic information about your Helm releases, including revision number, deployment date, release message, cluster details, and deployment status.
![Detail6](images/screenshot_basic_info.png)

### Resource Tab

In the Resources tab of the Helm Dashboard, you can view the kind (type), name, status, and any associated messages for your Kubernetes resources.
![Detail7](images/screenshot_resource.png)

### Manifest Tab

Text: The Manifests tab displays the textual representation of the Kubernetes manifests associated with your Helm release. It provides the YAML or JSON configuration files that define the desired state of the resources deployed in your cluster.
![Detail8](images/screenshot_manifest_view.png)

Diff with Previous: The "Diff with Previous" feature allows you to compare the current version of the manifests with the previous version. It highlights the differences between the two versions, making it easier to identify the changes made in the deployment.
![Detail9](images/screenshot_manifest_diff_prev.png)

Diff with Specific: The "Diff with Specific" option enables you to compare the current version of the manifests with a specific past version. It allows you to select a particular revision and view the differences between that revision and the current one.
![Detail10](images/screenshot_manifest_diff_specific.png)

### Values Tab

Text: The Values tab displays the textual representation of the values file associated with your Helm chart. It shows the YAML or JSON file that contains the configuration values used during the deployment of the chart.
![Detail11](images/screenshot_values_view.png)

Diff: The "Diff" feature allows you to compare the current values with the previous values used in a previous deployment. It highlights any differences between the two versions, making it easier to identify changes made to the configuration.
![Detail12](images/screenshot_values_diff_prev.png)

### Text Tab

Text: The Notes tab displays any accompanying notes or documentation related to the Helm chart.
![Detail14](images/screenshot_notes_view.png)

Diff with previous: The "Diff" feature is not typically available in the Notes tab. This tab is primarily meant for viewing the static text-based notes associated with the chart and doesn't involve comparisons or tracking changes like in the Manifests or Values tabs.
![Detail15](images/screenshot_notes_diff_prev.png)

Diff with Specific Version: Similar to the previous point, the ability to view a diff with a specific version of the notes is not a standard feature in the Notes section of the Helm Dashboard. The Notes section usually presents the information for the specific version of the Helm chart that is currently deployed.
![Detail16](images/screenshot_notes_diff_specific_version.png)










