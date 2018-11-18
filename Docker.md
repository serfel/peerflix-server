Docker
========

`docker pull serfel/peerflix-server-rus`

Make sure that you have write permissions to your destination directory `/tmp/torrent-stream`:

```sh
mkdir /tmp/torrent-stream
chmod a+rw /tmp/torrent-stream/
```

`docker run -p 9000:9000 -p 6881:6881 -p 6881:6881/udp -d -v /tmp/torrent-stream:/tmp/torrent-stream serfel/peerflix-server-rus`

Or

`docker run -p 9000:9000 -p 6881:6881 -p 6881:6881/udp --rm -v /tmp/torrent-stream:/tmp/torrent-stream serfel/peerflix-server-rus`
