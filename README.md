### Good reads:
1. Difference between the "images" fields in Cloudbuild and using Docker push comes down to seeing details about the images that were built by Cloudbuild in the logs. "https://cloud.google.com/cloud-build/docs/configuring-builds/store-images-artifacts"

2. Knative traffic splitting: https://github.com/meteatamel/knative-tutorial/blob/master/docs/04-trafficsplitting.md

3. Medium hands-on Knative series:
    * https://medium.com/google-cloud/hands-on-knative-part-1-f2d5ce89944e
    * https://medium.com/google-cloud/hands-on-knative-part-2-a27729f4d756
    * https://medium.com/google-cloud/hands-on-knative-part-3-d8731ad2f23d
    * https://medium.com/knative/knative-v0-3-autoscaling-a-love-story-d6954279a67a
    * Great step by step tutorial: https://github.com/meteatamel/knative-tutorial/blob/master/docs/01-helloworldserving.md


4. Github Knative site: https://github.com/knative

5. Youtube video offering a good short overview of Knative: https://www.youtube.com/watch?v=Xi9oYTR710E&t=35s

6. Git cmds to remember:
    * Create a new branch:
    * >git checkout -b knative
    * Edit, add and commit your files.
    * Push your branch to the remote repository:
    * >git push -u google knative

7. Create service accounts for pulling code from Google Source Repositories 

8. Install custom builders and build templates before using them.

9. Ensure correct /workspace/folder-name/Dockerfile" is used.

10. How to install community builders: https://github.com/googlecloudplatform/cloud-builders-community

11. convert a file to base64 and format output to single line.
       > cat known_hosts | base64 | tr -d '\n'

12. create ssh key pairs without password:
 > ssh-keygen -t rsa -b 4096 -C "ronaldboodram@google.com"

13. Add ssh to ssh-agent:
> eval "$(ssh-agent -s)"

> ssh-add ~/.ssh/id_rsa

14. convert ssh and known_hosts file to base64 and create secret and serviceaccount

15. https://help.github.com/en/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

16. https://github.com/knative/build/blob/master/test/git-ssh/2-build.yaml

17. "Cloud Platform" API needs to be enabled inorder to access GCR without authenticating

18. knative cmds in kubectl:
       * kubectl get builds, will list all builds
       * kubectl delete builds --all, will delete all builds
       * kubectl get ksvc, will list all knative services
       * kubectl delete ksvc --all, will delete all knative services







