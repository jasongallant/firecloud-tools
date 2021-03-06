## List and delete Dataproc clusters across projects
This script will query Google projects for old Dataproc clusters and optionally call deletion APIs.

Prerequisites: the [Google Cloud SDK](https://cloud.google.com/sdk/) and a Firecloud Test Domain Admin or Quality 
Domain Admin user.  Before running this script, log in as that user: `gcloud auth login <email>`

Usage (from the main directory):

```./cleanup_clusters/cleanup_clusters.sh [list|delete] log_suffix```

`list` will print out the list of old clusters but not delete them.  `delete` will actually delete them.

`log_suffix` is a string (example: QA) to include in the log file name to distinguish it from other runs on the same day.
