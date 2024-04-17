Requires NFS shares to be mounted on the docker hosts

sudo mount 10.20.30.11:/volume2/test/navidrome_data /nfs/navidrome_data
sudo mount 10.20.30.11:/volume2/test/navidrome_music /nfs/navidrome_music
# can that be RO on the music? 

Making changes requires; # otherwise container seems to cache something. 
docker-compose down
docker-compose up

Substreamer android app seems ok for connecting. 
Needs http only connection, legacy auth. dont share passwords.
