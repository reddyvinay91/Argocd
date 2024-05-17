<ins>Task 1 (Setup and configuration)</ins>
<br/>

1) I had setup the gito repo in git UI , cloned the repo. <br/>
2) Ensured the complete setup of minikube is done and working fine.<br/>
   <ins>Challenges</ins>: Encountered issues while installing minikube and setting up, but resolved them.

3) Read the documentation of argocd and argo rollout controllers and installed them and ensured argocd
   setup is working fine.

<ins>Task2 (Creating GitOps Pipeline )</ins>
<br/>
1) Initially i had developed a flask app as a web application in a seperate feature, but stopped using it<br/>
2) Then, developed an application called first-app which has simple deployment and service yaml files.<br/>
3) Here, i also understood argocd architecture and how all services are used inside.<br/>
4) I ensured argocd-server port is open and accessible in web-browser, so that i can use argocd-ui.<br/>
5) Using the http url of argocd-server POD, i accessed the ui (https://127.0.0.1:51689/)<br/>
6) Then in UI, i created the application, specifying all the fields and then argocd pipeline is setup.<br/>
7) Then as part of testing, i pushed some change to check whether argocd is working or not and it <br/>
   reflected that change automatically in the application.<br/>


<ins>Task 3 (Implementing a Canary Release with Argo Rollouts)</ins> <br/>
1)First understood, what is canary release<br/>
2)Later developed an application (rollout-app) with basic yaml files.<br/>
3)In the argocd ui, creation another application using rollout code, ensured gitops pipeline is setup 
  over there.<br/>
4)Later, i have the changed the container image version and using certain kubectl commands , i am able 
  to check rollout strategy is working.<br/>
5)Then, i have the completed the argocd tasks.<br/>

<ins>Task 4(Documentation &cleanup)==</ins> <br/>
1)Documentation is done in this readme file itself<br/>
2)I have not done the cleanup ,  but i have read the documentation on how to clear the resources in the 
  kubernetes cluster<br/>
  some of the commands used in cleanup are:<br/>
    kubectl delete deployments --all<br/>
    kubectl delete services --all<br/>
    kubectl delete pods --all<br/>
    kubectl delete daemonset --all<br/>