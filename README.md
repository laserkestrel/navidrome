Requires NFS shares to be mounted on the docker hosts<br>
<br>
/etc/fstab<br>
<NASIP>:/volume2/test/navidrome_data /nfs/navidrome_data nfs auto,nofail,noatime,nolock,intr,tcp,actimeo=1800 0 0<br>
<NASIP>:/volume2/test/navidrome_music /nfs/navidrome_music nfs auto ro,nofail,noatime,nolock,intr,tcp,actimeo=1800 0 0<br>
<br>
Making changes requires; # otherwise container seems to cache something. <br>
docker-compose down<br>
docker-compose up<br><br>

Substreamer android app seems ok for connecting. <br>
Needs http only connection, legacy auth. dont share passwords.<br>

