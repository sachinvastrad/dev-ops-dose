# step 1: install oracle virtual box //https://www.virtualbox.org/wiki/Downloads
# step2 : open powershell
# step3: run this command " Get-ExecutionPolicy" If it returns Restricted, then run Set-ExecutionPolicy AllSigned or Set-ExecutionPolicy Bypass -Scope Process.

## Install Chocolatey
# step 4: run command " Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1')) "
# step 5: Add to environment PATH variable  e,g  C:\ProgramData\chocolatey\bin
# step 6: check choco version

 ### PS C:\Windows\system32> choco
 ###  Chocolatey v0.10.15Please run 'choco -?' or 'choco <command> -?' for help menu.
 ###  PS C:\Windows\system32>
# step 7: choco install kubernetes-cli
# Step 8: install minikube     https://github.com/kubernetes/minikube/releases
## once you down load exe 
## create a DIR in e.g  C:\k8 and copy-paste the downloaded file

## minikube.exe start  ( name of the Exe which you download)

## RUN a command to check setup is allgood  :

# kubectl  run -it sachin-pod --image=ubuntu --restart=Never -- bash

### This should spin the pod named sachin-pod on you machine and put in bash shell

## To exit shell press ctrl+ c 


