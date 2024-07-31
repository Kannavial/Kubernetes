Saya disini hanya mengubah 2 variabel, 
  Variable selector.matchLabels yang berisi debug-apps menjadi debug-app.
  Variable resources.limits dan resources.requests untuk lebih besar dimana sebelumnya resource.limits lebih kecil daripada yang di request. 
Kesusahan saya disini mencari masalahnya, seperti biasa saya baca pelan-pelan dari atas sampai bawah, Saya melihat ada variable yang salah (selector.matchLabels) dengan ikonsistensi dalam penamaan dan resource.limits yang besarnya 1/2 daripada request. 

Command yang di run:
  kubectl apply -f debug-deployment.yaml
  kubectl get deployments
  kubectl get pods
  kubectl describe deployment debug-deployment

