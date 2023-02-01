# docker_basics
installer docker https://docs.docker.com/

télécharger une image nginx (nginx:serveur d'execution des app statique): docker pull nginx

exécuter l'image: docker run nginx

exporter le port sur 8080: docker run -p 8080:80 nginx  //on peut remplacer le nom d'image avec l'id 

exécuter limage en arrier plan:docker run -tdi -p8080:80 nginx //tdi :(t allouer un terminal virturl/i:garder l'entree clavier/d:executer le contenue

changer le nom du conteneur :
docker rm -f id-conteneur (supprimer )
docker run -tdi -p 8080:80 -v --name aaaaa nginx
 
 pour avoir tous les conteneur : docker ps -a
 pour avour les conteneur actif : docker ps 
 
 
 entrer dans le conteneur 
 docker exec -it id-conteneur /bin/bash OUBIEN docker exec -it id-conteneur sh
 
 
 pou modifier le contenue de fichier 
 ls 
 cd /usr/share/nginx/html/
 cat index.html
    
    
    apt update && install vim 
    
    
    ajouter le volume d' une page index personalisé a notre conteneur
    docker run -tdi -p 8080:80 -v C:/Users/Eya/OneDrive/Bureau/DOCKER/nginx/:/usr/share/nginx/html/ --name aaaaa a99a39d070bf
    
 
 
 
 
 
 


