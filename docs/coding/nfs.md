# Créer un partage NFS

### But : partager le volume /dev/vg-data/lv-nfs pour y accéder à partir d’un client Linux.

### Étape 1 :

```installation title="Installer le serveur NFS"

apt-get update
apt-get install nfs-kernel-server
```

### Étape 2 :

```Monter-le-volume title="Monter le volume et créer le répertoire à partager"

mount /dev/vg-data/lv-nfs /mnt/nfs
mkdir /mnt/nfs/partage
```

### Étape 3 :

```Configurer title="Configurer le serveur NFS"
nano /etc/exports
Ajouter la ligne suivante à la fin du fichier :
/mnt/nfs/partage \*(rw,no_root_squash)
```

### Étape 4 :

```Redémarrer title="Redémarrer le serveur NFS"
service nfs-kernel-server restart
```
