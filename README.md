# devops_final_jenkins_retake_20250715


Jenkins Development:
_1.	Make a pipeline named base pipeline
_a.	Should be triggered when merge request is accepted from dev -> main branch.
_b.	Upon merge acceptance pipeline is triggered
c.	Git code is pulled
d.	Docker image is built
i.	Image tag should be: pipeline_build_number-day-month-hour-minute
e.	Docker push to dockerhub (using username and password variable from the jenkins credentials)
f.	Docker logout
g.	Clean the workspace
h.	Use linux commands to update the image tag at dockercompose.yaml file in the /var/www/app directory
i.	After updating the docker compose file, rerun the docker compose so that the container picks the new image and start with the new image.
j.	Send a google chat notification (if pipeline successful)
i.	Notification should be “your application has been updated, Imagename:imagetag”			
k.	Push the code to the repository
