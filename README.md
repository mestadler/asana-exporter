# asana-exporter
Export your Asana data in json or csv

Python3 script to export your Asana data with an your API key either to back up or to convert for use with other applications.  The csv export is functional but still experimental, as it does not propoerly parse the subtask stories.  

* Can list your teams and projects
* Can export your projects and export your teams (all projects in a team)
* You can generate a personal access token from the Asana developer console, https://app.asana.com/0/my-apps you will need this to use the asana-exporter.
* If you run without any arguments, will export your whole asana data in json format.

Usage: asana-export [-h] --token TOKEN [--query {teams,projects}] [--format {json,csv}] [--team_name TEAM_NAME] [--project_name PROJECT_NAME]

Export Asana data to JSON or CSV.

options:
  -h, --help            show this help message and exit
  --token TOKEN         Your Asana Personal Access Token
  --query {teams,projects}
                        Query for available teams or projects
  --format {json,csv}   Export format: json or csv
  --team_name TEAM_NAME
                        Name of the team you want to filter by
  --project_name PROJECT_NAME
                        Name of the project you want to filter by

