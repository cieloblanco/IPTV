
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
                            
CANALES - m3u8
  #EXTM3U
  #EXTINF:0,TvPerúHD,/home/vlue/Pictures/TV_Perú_HD.png,0
  rtmp://cdnp2.iblups.com/tvperuhd/ playpath=R9WtilpKKB swfUrl=https://iblups.com/jw7/jwplayer.flash.swf live=1 pageUrl=https://iblups.com/e_tvperuHD
  #EXTINF:0,PanamericanaTV,/home/vlue/Pictures/panamericana tv.png,0
  rtmp://cdnp5.iblups.com/ptv/ playpath=ptv swfUrl=https://iblups.com/jw7/jwplayer.flash.swf live=1 pageUrl=https://iblups.com/e_panamericanatv
  #EXTINF:0,Latina 1500kbps,/home/vlue/Pictures/Latina_Television.jpg,0
  http://cialive-live.hds.adaptive.level3.net/hls-live/ciaremux-live/_definst_/live/stream4.m3u8
  #EXTINF:0,WillaxHD,/home/vlue/Pictures/willaxTv-logo.jpg,0
  rtmp://willax.mediastream.pe/ app=vv_willax playpath=livestream swfUrl=http://monitor.mediastream.pe/MStreamLive.swf?v=qtnjVOvh pageUrl=http://willax.tv/ live=true
  #EXTINF:0,RBC,/home/vlue/Pictures/RBC-Satelital.jpg,0
  rtmp://184.154.28.210:1935/rbc-tv/ playpath=rbc-tv swfUrl=http://www.servistream.pe/players-tv/jwplayer/jwplayer.flash.swf pageUrl=http://www.rbconline.pe/ live=1 swfVfy=true
  #EXTINF:0,MegaTV Aqp,/home/vlue/Pictures/megatv2.jpg,0
  rtmp://play.hostreamperu.com:1935/ app=8016/ playpath=8016 swfUrl=http://ssl.p.jwpcdn.com/player/v/7.8.6/jwplayer.flash.swf pageUrl=http://www.megatvarequipa.com/megatvarequipa-live/ live=1 swfVfy=true
  #EXTINF:0,SolTv LaLibertad,/home/vlue/Pictures/soltv-peru.png,0
  rtmp://wowzaserver.net:1935/vivo21/ playpath=vivo21 swfUrl=http://p.jwpcdn.com/6/12/jwplayer.flash.swf pageUrl=http://www.soltvperu.com/envivo.html live=1 swfVfy=true
  #EXTINF:0,CapitalTV,/home/vlue/Pictures/capitaltv.jpg,0
  http://streaming.video.webrpp-live.hls.adaptive.level3.net/hls-live/videoremux-videoCAPTV/_definst_/live.m3u8
  #EXTINF:0,LaLuz,/home/vlue/Pictures/laluz.png,0
  http://stream.iglesiaytecnologia.com:2077/live/tvlaluz/playlist.m3u8
  #EXTINF:0,Pax,/home/vlue/Pictures/pax.png,0
  http://d2s2gdjgdcyicj.cloudfront.net/paxtv/smil:PC.smil/playlist.m3u8
  #EXTINF:0,AnimeTV,,0
  http://video7.stream.mx:1935/raxatv/raxatv/chunklist_w884577146.m3u8

