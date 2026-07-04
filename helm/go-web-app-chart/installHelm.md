# for ubuntu linux

curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-4

chmod 700 get_helm.sh
./get_helm.sh

# check installation
helm version

# create a helm chart using command 

helm  create go-web-app-chart ("go-web-app-chart" replace anything name)




# how to install anything using helm command 
helm install go-web-app ./go-web-app-chart



