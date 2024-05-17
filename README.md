==Task 1 (Setup and configuration)==

1) I had setup the gito repo in git UI , cloned the repo.
2) Ensured the complete setup of minikube is done and working fine.
   <ins>Challenges</ins>: Encountered issues while installing minikube and setting up, but resolved them.

3) Read the documentation of argocd and argo rollout controllers and installed them and ensured argocd
   setup is working fine.

==Task2 (Creating GitOps Pipeline )==
1) Initially i had developed a flask app as a web application in a seperate feature, but stopped using it
2) Then, developed an application called first-app which has simple deployment and service yaml files.
3) Here, i also understood argocd architecture and how all services are used inside.
4) I ensured argocd-server port is open and accessible in web-browser, so that i can use argocd-ui.
5) Using the http url of argocd-server POD, i accessed the ui (https://127.0.0.1:51689/)
6) Then in UI, i created the application, specifying all the fields and then argocd pipeline is setup.
7) Then as part of testing, i pushed some change to check whether argocd is working or not and it 
   reflected that change automatically in the application.


==Task 3 (Implementing a Canary Release with Argo Rollouts)==
1)First understood, what is canary release
2)Later developed an application (rollout-app) with basic yaml files.
3)In the argocd ui, creation another application using rollout code, ensured gitops pipeline is setup 
  over there.
4)Later, i have the changed the container image version and using certain kubectl commands , i am able 
  to check rollout strategy is working.
5)Then, i have the completed the argocd tasks.

==Task 4(Documentation &cleanup)==
1)Documentation is done in this readme file itself
2)I have not done the cleanup ,  but i have read the documentation on how to clear the resources in the 
  kubernetes cluster
  some of the commands used in cleanup are:
    kubectl delete deployments --all
    kubectl delete services --all
    kubectl delete pods --all
    kubectl delete daemonset --all