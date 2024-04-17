Requires NFS shares to be mounted on the docker hosts<br>
<br>
sudo mount 10.20.30.11:/volume2/test/navidrome_data /nfs/navidrome_data<br>
sudo mount 10.20.30.11:/volume2/test/navidrome_music /nfs/navidrome_music<br>
# can that be RO on the music? <br><br>

Making changes requires; # otherwise container seems to cache something. 
docker-compose down<br>
docker-compose up<br><br>

Substreamer android app seems ok for connecting. <br>
Needs http only connection, legacy auth. dont share passwords.<br>
