# MartiniqueALaCarte
##Process pour que les modifications apparaissent sur le site automatquement :
1) faire les modifications souhaitées sur les html
2) Actualiser le statefullset.yaml avec la version voulue de l'image cf  site_martinique:v5 
3) Actualiser le github/workflows/docker-publish.yaml avec la bonne version egalement pendant le docker push site_martinique:v5 (v5 désigne en fait un tag)
4) git add/commit/push
5) Attendre moins de 5 min  :)

## Regesx pour remplacer tpus les blabla.jpg en img/blabla.jpg
recherche regex : (\w+)(?=\.jpg) 
remplacement : img/$1  
$1 désigne lme premeir groupe attaché à la Regex
