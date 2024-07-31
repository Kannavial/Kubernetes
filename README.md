# Saya disini hanya mengubah 3 variabel, 
  1. Variable selector.matchLabels yang berisi debug-apps menjadi debug-app.
  2. Variable resources.limits dan resources.requests untuk lebih besar dimana sebelumnya resource.limits lebih kecil daripada yang di request.
  3. Variable untuk path /healthz dikarenakan endpointnya tidak ada
> Kesusahan saya disini mencari masalahnya, seperti biasa saya baca pelan-pelan dari atas sampai bawah, Saya melihat ada variable yang salah (selector.matchLabels) dengan ikonsistensi dalam penamaan dan resource.limits yang besarnya 1/2 daripada request. Untuk path /healthz itu cukup membingungkan karena saya tidak melewati itu. 

# Command yang di run:
  1. kubectl apply -f debug-deployment.yaml
  2. kubectl get deployments
  3. kubectl get pods
  4. kubectl describe deployment debug-deployment

