
FUENTE DE EMISIÓN
  IPTV
    http://blog.exabytetv.info/listas/
  LOCAL STREAMING    
      Acestream
        emisión             #duplicate{dst="http{mux=ts,dst=:8903/tv.asf}",dst=display}
        caché               15000
        engine              Start with sufficient speed only
        engine puerto       8621 
        
REPRODUCTOR
      URL                   http://192.168.y.x:8902/tv.asf
      M3U                   https://raw.githubusercontent.com/k-st/IPTV/master/IP_Nro_x.m3u
      PLEX
plugin https://github.com/Cigaras/IPTV.bundle
