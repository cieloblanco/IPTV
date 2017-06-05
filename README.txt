
FUENTE DE EMISIÓN
  IPTV
    http://blog.exabytetv.info/listas/
  LOCAL STREAMING    
      Acestream
        emisión             #duplicate{dst="http{mux=ts,dst=:8902/tv.asf}",dst=display}
        caché(ms)           15000
        engine              https://raw.githubusercontent.com/k-st/IPTV/master/engine.png 
        
REPRODUCTOR
      URL                   http://192.168.Y.X:8902/tv.asf
      PLEX
        plugin           
          instalarlo (pegar)
                            https://github.com/Cigaras/IPTV.bundle
                            windows   C:\Users\usuario\AppData\Local\Plex Media Server\Plug-ins
                            ubuntu    /var/lib/plexmediaserver/Library/Application Support/Plex Media Server/Plug-ins
          agregar el contenido de "https://raw.githubusercontent.com/k-st/IPTV/master/linea_m3u" a "/var/lib/.../Resources/playlist.m3u", cambiando valores de Y y X
                            
CANALES

  TvPerúHD
    rtmp://cdnp2.iblups.com/tvperuhd/ playpath=R9WtilpKKB swfUrl=https://iblups.com/jw7/jwplayer.flash.swf live=1 pageUrl=https://iblups.com/e_tvperuHD
  PanamericanaTV HD
    rtmp://cdnp5.iblups.com/ptv/ playpath=ptv swfUrl=https://iblups.com/jw7/jwplayer.flash.swf live=1 pageUrl=https://iblups.com/e_panamericanatv
  Latina 1500kbps
    http://cialive-live.hds.adaptive.level3.net/hls-live/ciaremux-live/_definst_/live/stream4.m3u8
