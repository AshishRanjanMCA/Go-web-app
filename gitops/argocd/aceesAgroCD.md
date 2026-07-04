# ArgoCD user is : Admin

# how to get passord of argocd
    kubectl get secret argocd-initial-admin-secret -n argocd -o jsonpath="{.data.password}" | base64 -d
    echo


# How to setup argocd to our git
  1. go to application 
  2. click on new app
  3. application give anything like (go-web-app)
  4. project name ->Default
  5. SYNC Policy --> choose Automatic -->enable  Auto syn and self Heal
  6. Source --> give your git repo url where   is  your application is available.
    
    a.Repository url :https://github.com/AshishRanjanMCA/Go-web-app.git

    b. Revision --> main
    c. Path -->helm/go-web-app-chart
  

  7. DESTINATION

     Cluster url 
         https://kubernetes.default.svc
    
    NameSpace:
      default
     