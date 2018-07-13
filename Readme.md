## Kubernetes Demo

### Instructions

* Install minkube, if you do not already have it installed:

        brew cask install minikube
    
* Start `minikube`
        
        minikube start

* Check that `kubectl` is setup correctly

        kubectl get nodes

* Create the `deployment`

        kubectl apply -f deployment.yml

* Create the `service`

        kubectl apply -f service.yml

* Test out the deployed service in a brower

        minkube service k8-session

* Change the number of pods running

        kubectl scale deployment k8-session --replicas=1

* Shutdown minikube when you are done

        minikube stop