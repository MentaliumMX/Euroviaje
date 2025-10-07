# Euroviaje
El viaje de nuestras vidas
<!DOCTYPE html>
<html>
<head>
    
    <meta http-equiv="content-type" content="text/html; charset=UTF-8" />
    
        <script>
            L_NO_TOUCH = false;
            L_DISABLE_3D = false;
        </script>
    
    <style>html, body {width: 100%;height: 100%;margin: 0;padding: 0;}</style>
    <style>#map {position:absolute;top:0;bottom:0;right:0;left:0;}</style>
    <script src="https://cdn.jsdelivr.net/npm/leaflet@1.6.0/dist/leaflet.js"></script>
    <script src="https://code.jquery.com/jquery-1.12.4.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/js/bootstrap.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/Leaflet.awesome-markers/2.0.2/leaflet.awesome-markers.js"></script>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/leaflet@1.6.0/dist/leaflet.css"/>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap.min.css"/>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap-theme.min.css"/>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.6.3/css/font-awesome.min.css"/>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/Leaflet.awesome-markers/2.0.2/leaflet.awesome-markers.css"/>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/python-visualization/folium/folium/templates/leaflet.awesome.rotate.min.css"/>
    
            <meta name="viewport" content="width=device-width,
                initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
            <style>
                #map_0ed7fbc329ef96a2cc8a6e169afeb65c {
                    position: relative;
                    width: 100.0%;
                    height: 100.0%;
                    left: 0.0%;
                    top: 0.0%;
                }
            </style>
        
    <script src="https://cdnjs.cloudflare.com/ajax/libs/leaflet.markercluster/1.1.0/leaflet.markercluster.js"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/leaflet.markercluster/1.1.0/MarkerCluster.css"/>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/leaflet.markercluster/1.1.0/MarkerCluster.Default.css"/>
    <script src="https://cdn.jsdelivr.net/npm/leaflet-ant-path@1.1.2/dist/leaflet-ant-path.min.js"></script>
</head>
<body>
    
    
            <div class="folium-map" id="map_0ed7fbc329ef96a2cc8a6e169afeb65c" ></div>
        
</body>
<script>
    
    
            var map_0ed7fbc329ef96a2cc8a6e169afeb65c = L.map(
                "map_0ed7fbc329ef96a2cc8a6e169afeb65c",
                {
                    center: [50.0, 12.0],
                    crs: L.CRS.EPSG3857,
                    zoom: 5,
                    zoomControl: true,
                    preferCanvas: false,
                }
            );

            

        
    
            var tile_layer_852ca5e45a19036c94569da1fa9db7e1 = L.tileLayer(
                "https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",
                {"attribution": "Data by \u0026copy; \u003ca href=\"http://openstreetmap.org\"\u003eOpenStreetMap\u003c/a\u003e, under \u003ca href=\"http://www.openstreetmap.org/copyright\"\u003eODbL\u003c/a\u003e.", "detectRetina": false, "maxNativeZoom": 18, "maxZoom": 18, "minZoom": 0, "noWrap": false, "opacity": 1, "subdomains": "abc", "tms": false}
            ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
    
            var feature_group_9c4018803c0833d32cfb204e7660df45 = L.featureGroup(
                {}
            ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
    
            var marker_285b9822efaf8bca688a1c51a0503582 = L.marker(
                [40.4168, -3.7038],
                {}
            ).addTo(feature_group_9c4018803c0833d32cfb204e7660df45);
        
    
            var icon_dc45041f2f04b848003d9b488dc39421 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "info-sign", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_285b9822efaf8bca688a1c51a0503582.setIcon(icon_dc45041f2f04b848003d9b488dc39421);
        
    
        var popup_bac1688e3ef650763d0eeb61c04d0647 = L.popup({"maxWidth": 320});

        
            var i_frame_689bc5d81ca743ce40b2b68de8b0c1b9 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgIDxkaXYgc3R5bGU9J2ZvbnQtZmFtaWx5OiBBcmlhbCwgc2Fucy1zZXJpZjsgd2lkdGg6IDI2MHB4Jz4KICAgICAgICA8aDQgc3R5bGU9J21hcmdpbjowIDAgNnB4IDAnPjEuIE1hZHJpZDwvaDQ+CiAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz48Yj5Fc3RhbmNpYTo8L2I+IDE04oCTMTcgb2N0PC9wPgogICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+PGI+TGxlZ2FkYTo8L2I+IDE0IG9jdCwgMTg6MzA8L3A+CiAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz48Yj5TYWxpZGE6PC9iPiAxNyBvY3QsIDEzOjA1PC9wPgogICAgICAgIDxwIHN0eWxlPSdtYXJnaW46NnB4IDAgMCAwJz5Ub2NhIGxvcyBtYXJjYWRvcmVzIGNlcmNhbm9zIHBhcmEgdmVyIGxvcyBwdW50b3MgZGUgaW50ZXLDqXMuPC9wPgogICAgPC9kaXY+CiAgICA=" width="300" style="border:none !important;" height="160"></iframe>`)[0];
            popup_bac1688e3ef650763d0eeb61c04d0647.setContent(i_frame_689bc5d81ca743ce40b2b68de8b0c1b9);
        

        marker_285b9822efaf8bca688a1c51a0503582.bindPopup(popup_bac1688e3ef650763d0eeb61c04d0647)
        ;

        
    
    
            marker_285b9822efaf8bca688a1c51a0503582.bindTooltip(
                `<div>
                     1. Madrid (resumen)
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_cluster_119cdc768972491c63433af6bd0999e9 = L.markerClusterGroup(
                {}
            );
            feature_group_9c4018803c0833d32cfb204e7660df45.addLayer(marker_cluster_119cdc768972491c63433af6bd0999e9);
        
    
            var marker_ab11a01d59fd0406292fa8434342e51e = L.marker(
                [40.4138, -3.6921],
                {}
            ).addTo(marker_cluster_119cdc768972491c63433af6bd0999e9);
        
    
            var icon_64629156d063d123c26d64e4cdd9b438 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_ab11a01d59fd0406292fa8434342e51e.setIcon(icon_64629156d063d123c26d64e4cdd9b438);
        
    
        var popup_232f07ee37c348062499a8d5717c3f8b = L.popup({"maxWidth": 280});

        
            var i_frame_8d05d769edd5447aaceca966ee1e175e = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+TXVzZW8gZGVsIFByYWRvPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IE1hZHJpZDwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_232f07ee37c348062499a8d5717c3f8b.setContent(i_frame_8d05d769edd5447aaceca966ee1e175e);
        

        marker_ab11a01d59fd0406292fa8434342e51e.bindPopup(popup_232f07ee37c348062499a8d5717c3f8b)
        ;

        
    
    
            marker_ab11a01d59fd0406292fa8434342e51e.bindTooltip(
                `<div>
                     Museo del Prado
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_59f3904fdfcfca7898f5d37cc854dfef = L.marker(
                [40.4153, -3.6844],
                {}
            ).addTo(marker_cluster_119cdc768972491c63433af6bd0999e9);
        
    
            var icon_6fa31777463b503b9d4c87ebe4e9ed13 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_59f3904fdfcfca7898f5d37cc854dfef.setIcon(icon_6fa31777463b503b9d4c87ebe4e9ed13);
        
    
        var popup_a57046cdf85b4197532b3ddb0c91a604 = L.popup({"maxWidth": 280});

        
            var i_frame_7574b733d0849200a3bc80e2a71120df = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UGFycXVlIGRlbCBSZXRpcm88L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogTWFkcmlkPC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_a57046cdf85b4197532b3ddb0c91a604.setContent(i_frame_7574b733d0849200a3bc80e2a71120df);
        

        marker_59f3904fdfcfca7898f5d37cc854dfef.bindPopup(popup_a57046cdf85b4197532b3ddb0c91a604)
        ;

        
    
    
            marker_59f3904fdfcfca7898f5d37cc854dfef.bindTooltip(
                `<div>
                     Parque del Retiro
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_9b5f531718d7e8e969be247f1902b0a2 = L.marker(
                [40.4203, -3.6883],
                {}
            ).addTo(marker_cluster_119cdc768972491c63433af6bd0999e9);
        
    
            var icon_12d6d75275987a25b9a25ca5ee3595e1 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_9b5f531718d7e8e969be247f1902b0a2.setIcon(icon_12d6d75275987a25b9a25ca5ee3595e1);
        
    
        var popup_0600f85c6fd5179a5271736e023590bd = L.popup({"maxWidth": 280});

        
            var i_frame_d6e559736c22e1298ab00a4380021e99 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UHVlcnRhIGRlIEFsY2Fsw6E8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogTWFkcmlkPC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_0600f85c6fd5179a5271736e023590bd.setContent(i_frame_d6e559736c22e1298ab00a4380021e99);
        

        marker_9b5f531718d7e8e969be247f1902b0a2.bindPopup(popup_0600f85c6fd5179a5271736e023590bd)
        ;

        
    
    
            marker_9b5f531718d7e8e969be247f1902b0a2.bindTooltip(
                `<div>
                     Puerta de Alcalá
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_fb2f941f544c003dd0871d5d59b0ad57 = L.marker(
                [40.419, -3.693],
                {}
            ).addTo(marker_cluster_119cdc768972491c63433af6bd0999e9);
        
    
            var icon_372fcfc484f78615078c73f7abafcb93 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_fb2f941f544c003dd0871d5d59b0ad57.setIcon(icon_372fcfc484f78615078c73f7abafcb93);
        
    
        var popup_b533c16c3246f779dc50eb513b082a57 = L.popup({"maxWidth": 280});

        
            var i_frame_9547db3499806d3fcf752d1b70c154c7 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UGxhemEgZGUgQ2liZWxlczwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBNYWRyaWQ8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_b533c16c3246f779dc50eb513b082a57.setContent(i_frame_9547db3499806d3fcf752d1b70c154c7);
        

        marker_fb2f941f544c003dd0871d5d59b0ad57.bindPopup(popup_b533c16c3246f779dc50eb513b082a57)
        ;

        
    
    
            marker_fb2f941f544c003dd0871d5d59b0ad57.bindTooltip(
                `<div>
                     Plaza de Cibeles
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_a90b29a9cb900019649e6402fdc9d3cb = L.marker(
                [40.4531, -3.6883],
                {}
            ).addTo(marker_cluster_119cdc768972491c63433af6bd0999e9);
        
    
            var icon_a0835384b95024aa96d6b535aca2f91b = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_a90b29a9cb900019649e6402fdc9d3cb.setIcon(icon_a0835384b95024aa96d6b535aca2f91b);
        
    
        var popup_55663307c64290d498fda92e05de7c76 = L.popup({"maxWidth": 280});

        
            var i_frame_1815b78f18420234838db3b4b04a700f = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+RXN0YWRpbyBTYW50aWFnbyBCZXJuYWLDqXU8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogTWFkcmlkPC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_55663307c64290d498fda92e05de7c76.setContent(i_frame_1815b78f18420234838db3b4b04a700f);
        

        marker_a90b29a9cb900019649e6402fdc9d3cb.bindPopup(popup_55663307c64290d498fda92e05de7c76)
        ;

        
    
    
            marker_a90b29a9cb900019649e6402fdc9d3cb.bindTooltip(
                `<div>
                     Estadio Santiago Bernabéu
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_d88429377127bb22adc7d59b73531dae = L.marker(
                [40.4203, -3.7058],
                {}
            ).addTo(marker_cluster_119cdc768972491c63433af6bd0999e9);
        
    
            var icon_46ec391b1fe53a3ca88405861d578d72 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_d88429377127bb22adc7d59b73531dae.setIcon(icon_46ec391b1fe53a3ca88405861d578d72);
        
    
        var popup_2963a5b53c643c6334c96342c5aa8e60 = L.popup({"maxWidth": 280});

        
            var i_frame_fffd2d410650df5bb6475ef3b8d99b2b = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+R3JhbiBWw61hPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IE1hZHJpZDwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_2963a5b53c643c6334c96342c5aa8e60.setContent(i_frame_fffd2d410650df5bb6475ef3b8d99b2b);
        

        marker_d88429377127bb22adc7d59b73531dae.bindPopup(popup_2963a5b53c643c6334c96342c5aa8e60)
        ;

        
    
    
            marker_d88429377127bb22adc7d59b73531dae.bindTooltip(
                `<div>
                     Gran Vía
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_3ff746a47bc0184e1f38fd2d544ae858 = L.marker(
                [40.424, -3.7184],
                {}
            ).addTo(marker_cluster_119cdc768972491c63433af6bd0999e9);
        
    
            var icon_7f273ff17314d58a00383744a2782527 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_3ff746a47bc0184e1f38fd2d544ae858.setIcon(icon_7f273ff17314d58a00383744a2782527);
        
    
        var popup_55f2006e6d264273a1f9bf34953c2d1e = L.popup({"maxWidth": 280});

        
            var i_frame_7fef958a04f1f30195966316185adf19 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+VGVtcGxvIGRlIERlYm9kPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IE1hZHJpZDwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_55f2006e6d264273a1f9bf34953c2d1e.setContent(i_frame_7fef958a04f1f30195966316185adf19);
        

        marker_3ff746a47bc0184e1f38fd2d544ae858.bindPopup(popup_55f2006e6d264273a1f9bf34953c2d1e)
        ;

        
    
    
            marker_3ff746a47bc0184e1f38fd2d544ae858.bindTooltip(
                `<div>
                     Templo de Debod
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_03c801b2c1650727d9fc0e97369c96e7 = L.marker(
                [40.411, -3.708],
                {}
            ).addTo(marker_cluster_119cdc768972491c63433af6bd0999e9);
        
    
            var icon_576557455071496c03b90f2010f8c035 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_03c801b2c1650727d9fc0e97369c96e7.setIcon(icon_576557455071496c03b90f2010f8c035);
        
    
        var popup_09adb6506e3ab59f208683577abf9ab1 = L.popup({"maxWidth": 280});

        
            var i_frame_e906c6c5157c336a28f6189d2616aa2b = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+TGEgTGF0aW5hPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IE1hZHJpZDwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_09adb6506e3ab59f208683577abf9ab1.setContent(i_frame_e906c6c5157c336a28f6189d2616aa2b);
        

        marker_03c801b2c1650727d9fc0e97369c96e7.bindPopup(popup_09adb6506e3ab59f208683577abf9ab1)
        ;

        
    
    
            marker_03c801b2c1650727d9fc0e97369c96e7.bindTooltip(
                `<div>
                     La Latina
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_11534919e770d2c90fd2a24a63b3c69f = L.marker(
                [40.4136, -3.6985],
                {}
            ).addTo(marker_cluster_119cdc768972491c63433af6bd0999e9);
        
    
            var icon_dc69cc095e8cc3179cb272c05129f8a0 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_11534919e770d2c90fd2a24a63b3c69f.setIcon(icon_dc69cc095e8cc3179cb272c05129f8a0);
        
    
        var popup_b6e3a5b909d35bc6f886f0bf760283d2 = L.popup({"maxWidth": 280});

        
            var i_frame_7e56db5a728e685016331980cc05e015 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+QmFycmlvIGRlIGxhcyBMZXRyYXM8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogTWFkcmlkPC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_b6e3a5b909d35bc6f886f0bf760283d2.setContent(i_frame_7e56db5a728e685016331980cc05e015);
        

        marker_11534919e770d2c90fd2a24a63b3c69f.bindPopup(popup_b6e3a5b909d35bc6f886f0bf760283d2)
        ;

        
    
    
            marker_11534919e770d2c90fd2a24a63b3c69f.bindTooltip(
                `<div>
                     Barrio de las Letras
                 </div>`,
                {"sticky": true}
            );
        
    
            var feature_group_43828e7afcbb140b68340dfa51cedb58 = L.featureGroup(
                {}
            ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
    
            var marker_44e4eec48e4e9d1890824eb924b13f68 = L.marker(
                [48.8566, 2.3522],
                {}
            ).addTo(feature_group_43828e7afcbb140b68340dfa51cedb58);
        
    
            var icon_8c9692f8e2e695fdd3c3a5b3361ac0f4 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "info-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_44e4eec48e4e9d1890824eb924b13f68.setIcon(icon_8c9692f8e2e695fdd3c3a5b3361ac0f4);
        
    
        var popup_35940114cfd7bbeb846fe3c4f3c70daa = L.popup({"maxWidth": 320});

        
            var i_frame_f95cb5793e68f264375b17ba7c9a9927 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgIDxkaXYgc3R5bGU9J2ZvbnQtZmFtaWx5OiBBcmlhbCwgc2Fucy1zZXJpZjsgd2lkdGg6IDI2MHB4Jz4KICAgICAgICA8aDQgc3R5bGU9J21hcmdpbjowIDAgNnB4IDAnPjIuIFBhcsOtczwvaDQ+CiAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz48Yj5Fc3RhbmNpYTo8L2I+IDE34oCTMjEgb2N0PC9wPgogICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+PGI+TGxlZ2FkYTo8L2I+IDE3IG9jdCwgMTU6MDU8L3A+CiAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz48Yj5TYWxpZGE6PC9iPiAyMSBvY3QsIDA5OjM1PC9wPgogICAgICAgIDxwIHN0eWxlPSdtYXJnaW46NnB4IDAgMCAwJz5Ub2NhIGxvcyBtYXJjYWRvcmVzIGNlcmNhbm9zIHBhcmEgdmVyIGxvcyBwdW50b3MgZGUgaW50ZXLDqXMuPC9wPgogICAgPC9kaXY+CiAgICA=" width="300" style="border:none !important;" height="160"></iframe>`)[0];
            popup_35940114cfd7bbeb846fe3c4f3c70daa.setContent(i_frame_f95cb5793e68f264375b17ba7c9a9927);
        

        marker_44e4eec48e4e9d1890824eb924b13f68.bindPopup(popup_35940114cfd7bbeb846fe3c4f3c70daa)
        ;

        
    
    
            marker_44e4eec48e4e9d1890824eb924b13f68.bindTooltip(
                `<div>
                     2. París (resumen)
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_cluster_1c1400456e39c1d77ad60e066754cb09 = L.markerClusterGroup(
                {}
            );
            feature_group_43828e7afcbb140b68340dfa51cedb58.addLayer(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var marker_5c55a94f074f6ec8ddad624636a1932f = L.marker(
                [48.853, 2.3499],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_7258fa416b101548aec6ac63cba6c051 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_5c55a94f074f6ec8ddad624636a1932f.setIcon(icon_7258fa416b101548aec6ac63cba6c051);
        
    
        var popup_b5aa633b9274160389a9695b56eede6e = L.popup({"maxWidth": 280});

        
            var i_frame_765de78f12b4b8df0fa7fee9a8ce79fe = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+Tm90cmUgRGFtZTwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBQYXLDrXM8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_b5aa633b9274160389a9695b56eede6e.setContent(i_frame_765de78f12b4b8df0fa7fee9a8ce79fe);
        

        marker_5c55a94f074f6ec8ddad624636a1932f.bindPopup(popup_b5aa633b9274160389a9695b56eede6e)
        ;

        
    
    
            marker_5c55a94f074f6ec8ddad624636a1932f.bindTooltip(
                `<div>
                     Notre Dame
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_9b244b68178e7b999457e856be4e7c4d = L.marker(
                [48.855, 2.345],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_287a36c6edb0833280ae0ce25606dfcc = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_9b244b68178e7b999457e856be4e7c4d.setIcon(icon_287a36c6edb0833280ae0ce25606dfcc);
        
    
        var popup_86d666bdd3999743b072a3c592dcc531 = L.popup({"maxWidth": 280});

        
            var i_frame_5746e9166c8a5023f4343b5ae7232c74 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+w45sZSBkZSBsYSBDaXTDqTwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBQYXLDrXM8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_86d666bdd3999743b072a3c592dcc531.setContent(i_frame_5746e9166c8a5023f4343b5ae7232c74);
        

        marker_9b244b68178e7b999457e856be4e7c4d.bindPopup(popup_86d666bdd3999743b072a3c592dcc531)
        ;

        
    
    
            marker_9b244b68178e7b999457e856be4e7c4d.bindTooltip(
                `<div>
                     Île de la Cité
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_b357e2d81244bec9b9407e66d4d04a70 = L.marker(
                [48.8493, 2.343],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_e34cc6e31622d9740c7fd31aa0455e95 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_b357e2d81244bec9b9407e66d4d04a70.setIcon(icon_e34cc6e31622d9740c7fd31aa0455e95);
        
    
        var popup_e6db8ce1d29eba7e13decbfa8721cbca = L.popup({"maxWidth": 280});

        
            var i_frame_fc93f6a7155c016696b5dbe05870a8e1 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+QmFycmlvIExhdGlubzwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBQYXLDrXM8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_e6db8ce1d29eba7e13decbfa8721cbca.setContent(i_frame_fc93f6a7155c016696b5dbe05870a8e1);
        

        marker_b357e2d81244bec9b9407e66d4d04a70.bindPopup(popup_e6db8ce1d29eba7e13decbfa8721cbca)
        ;

        
    
    
            marker_b357e2d81244bec9b9407e66d4d04a70.bindTooltip(
                `<div>
                     Barrio Latino
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_42059f324d1fae635134d146b75c5a88 = L.marker(
                [48.8462, 2.3459],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_f32f0fa37b6f39f85f1d4dad3ec8285c = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_42059f324d1fae635134d146b75c5a88.setIcon(icon_f32f0fa37b6f39f85f1d4dad3ec8285c);
        
    
        var popup_01e28a7f9e9a9e54cb6b3c7f4b3b1ee3 = L.popup({"maxWidth": 280});

        
            var i_frame_4bcc54e8c50d0519810922ff6f9a2b9d = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UGFudGXDs24gZGUgUGFyw61zPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFBhcsOtczwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_01e28a7f9e9a9e54cb6b3c7f4b3b1ee3.setContent(i_frame_4bcc54e8c50d0519810922ff6f9a2b9d);
        

        marker_42059f324d1fae635134d146b75c5a88.bindPopup(popup_01e28a7f9e9a9e54cb6b3c7f4b3b1ee3)
        ;

        
    
    
            marker_42059f324d1fae635134d146b75c5a88.bindTooltip(
                `<div>
                     Panteón de París
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_98feeed2a50f358efc81d5fb90dd4d09 = L.marker(
                [48.8462, 2.3371],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_73904b4593d954a147c71cfcac5a4672 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_98feeed2a50f358efc81d5fb90dd4d09.setIcon(icon_73904b4593d954a147c71cfcac5a4672);
        
    
        var popup_f20972c71575d934540b0c51f9454f16 = L.popup({"maxWidth": 280});

        
            var i_frame_eb3ebdb12ff621bc9496c1f667ea2156 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+SmFyZMOtbiBkZSBMdXhlbWJ1cmdvPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFBhcsOtczwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_f20972c71575d934540b0c51f9454f16.setContent(i_frame_eb3ebdb12ff621bc9496c1f667ea2156);
        

        marker_98feeed2a50f358efc81d5fb90dd4d09.bindPopup(popup_f20972c71575d934540b0c51f9454f16)
        ;

        
    
    
            marker_98feeed2a50f358efc81d5fb90dd4d09.bindTooltip(
                `<div>
                     Jardín de Luxemburgo
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_13dc09ac603eca226cfd29ce4dca212f = L.marker(
                [48.8628, 2.2871],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_b60fda0fc415ec3f355f9962cfc0c5db = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_13dc09ac603eca226cfd29ce4dca212f.setIcon(icon_b60fda0fc415ec3f355f9962cfc0c5db);
        
    
        var popup_f910c3a733ab9c79c01489f856c19c4b = L.popup({"maxWidth": 280});

        
            var i_frame_7cc40410466cd07487b6163717fbbca6 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+VHJvY2FkZXJvPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFBhcsOtczwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_f910c3a733ab9c79c01489f856c19c4b.setContent(i_frame_7cc40410466cd07487b6163717fbbca6);
        

        marker_13dc09ac603eca226cfd29ce4dca212f.bindPopup(popup_f910c3a733ab9c79c01489f856c19c4b)
        ;

        
    
    
            marker_13dc09ac603eca226cfd29ce4dca212f.bindTooltip(
                `<div>
                     Trocadero
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_49de86a30b04d4cda815fbf6f51b128c = L.marker(
                [48.8599, 2.3626],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_935e311990dd56f8a730e7a49c4bb59e = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_49de86a30b04d4cda815fbf6f51b128c.setIcon(icon_935e311990dd56f8a730e7a49c4bb59e);
        
    
        var popup_78866736173fa51a5963d0cf5e1eac02 = L.popup({"maxWidth": 280});

        
            var i_frame_6b9ff32ea5bbdd21ffdb2f2ab51e04e6 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+TGUgTWFyYWlzPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFBhcsOtczwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_78866736173fa51a5963d0cf5e1eac02.setContent(i_frame_6b9ff32ea5bbdd21ffdb2f2ab51e04e6);
        

        marker_49de86a30b04d4cda815fbf6f51b128c.bindPopup(popup_78866736173fa51a5963d0cf5e1eac02)
        ;

        
    
    
            marker_49de86a30b04d4cda815fbf6f51b128c.bindTooltip(
                `<div>
                     Le Marais
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_f6f539ced9b9a315e20ac114679019c3 = L.marker(
                [48.8867, 2.3431],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_32c57fff58b09fd4b9847d2f5a1cfb92 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_f6f539ced9b9a315e20ac114679019c3.setIcon(icon_32c57fff58b09fd4b9847d2f5a1cfb92);
        
    
        var popup_850456556f65f588f4341ad939d959c4 = L.popup({"maxWidth": 280});

        
            var i_frame_fff7268233347c849c7f18f4eea93ed9 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+U2FjcsOpLUPFk3VyPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFBhcsOtczwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_850456556f65f588f4341ad939d959c4.setContent(i_frame_fff7268233347c849c7f18f4eea93ed9);
        

        marker_f6f539ced9b9a315e20ac114679019c3.bindPopup(popup_850456556f65f588f4341ad939d959c4)
        ;

        
    
    
            marker_f6f539ced9b9a315e20ac114679019c3.bindTooltip(
                `<div>
                     Sacré-Cœur
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_b37c2bf019e1433418cb43cb98968280 = L.marker(
                [48.8862, 2.343],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_20c7a8f18efee4897421ebb09054027b = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_b37c2bf019e1433418cb43cb98968280.setIcon(icon_20c7a8f18efee4897421ebb09054027b);
        
    
        var popup_7ac46489911c6fc03fa41684ddfc2075 = L.popup({"maxWidth": 280});

        
            var i_frame_ed30e2d499ee94dcf1bd3398c21b1602 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UGxhY2UgZHUgVGVydHJlPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFBhcsOtczwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_7ac46489911c6fc03fa41684ddfc2075.setContent(i_frame_ed30e2d499ee94dcf1bd3398c21b1602);
        

        marker_b37c2bf019e1433418cb43cb98968280.bindPopup(popup_7ac46489911c6fc03fa41684ddfc2075)
        ;

        
    
    
            marker_b37c2bf019e1433418cb43cb98968280.bindTooltip(
                `<div>
                     Place du Tertre
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_2469cd150cb1c5971bfb4d043c25c992 = L.marker(
                [48.8841, 2.3324],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_448d87eca97d2c84c77bcfd4a157171a = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_2469cd150cb1c5971bfb4d043c25c992.setIcon(icon_448d87eca97d2c84c77bcfd4a157171a);
        
    
        var popup_3cbb33fbb8b1aa038ab56257e9b637bf = L.popup({"maxWidth": 280});

        
            var i_frame_4dc4b21c2036249b4c9401ff577fb367 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+TW91bGluIFJvdWdlPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFBhcsOtczwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_3cbb33fbb8b1aa038ab56257e9b637bf.setContent(i_frame_4dc4b21c2036249b4c9401ff577fb367);
        

        marker_2469cd150cb1c5971bfb4d043c25c992.bindPopup(popup_3cbb33fbb8b1aa038ab56257e9b637bf)
        ;

        
    
    
            marker_2469cd150cb1c5971bfb4d043c25c992.bindTooltip(
                `<div>
                     Moulin Rouge
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_f59efb0349d7583064dc606d7d6e3a67 = L.marker(
                [48.8719, 2.3316],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_023143f76b21ca533336b65a4ff2edc1 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_f59efb0349d7583064dc606d7d6e3a67.setIcon(icon_023143f76b21ca533336b65a4ff2edc1);
        
    
        var popup_18486518cf9d659ecd9c896ad4bccdfc = L.popup({"maxWidth": 280});

        
            var i_frame_1c5dc51f45a878c765cb1673e82d9cf5 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+w5NwZXJhIEdhcm5pZXI8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogUGFyw61zPC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_18486518cf9d659ecd9c896ad4bccdfc.setContent(i_frame_1c5dc51f45a878c765cb1673e82d9cf5);
        

        marker_f59efb0349d7583064dc606d7d6e3a67.bindPopup(popup_18486518cf9d659ecd9c896ad4bccdfc)
        ;

        
    
    
            marker_f59efb0349d7583064dc606d7d6e3a67.bindTooltip(
                `<div>
                     Ópera Garnier
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_d50e7812d5afb39f54a975491cd092a7 = L.marker(
                [48.8738, 2.3321],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_80916e399a69b7b41ee798e20f800b42 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_d50e7812d5afb39f54a975491cd092a7.setIcon(icon_80916e399a69b7b41ee798e20f800b42);
        
    
        var popup_69d7cad9b15879b2fd0d9737ef108743 = L.popup({"maxWidth": 280});

        
            var i_frame_53231a6bc8411697982388716f83d805 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+R2FsZXJpZXMgTGFmYXlldHRlPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFBhcsOtczwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_69d7cad9b15879b2fd0d9737ef108743.setContent(i_frame_53231a6bc8411697982388716f83d805);
        

        marker_d50e7812d5afb39f54a975491cd092a7.bindPopup(popup_69d7cad9b15879b2fd0d9737ef108743)
        ;

        
    
    
            marker_d50e7812d5afb39f54a975491cd092a7.bindTooltip(
                `<div>
                     Galeries Lafayette
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_d9dc2e0dc758b99c32ef5dfa5f09e52b = L.marker(
                [48.8698, 2.3073],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_95676faa93baa877d5b5ec8fdebcf3e0 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_d9dc2e0dc758b99c32ef5dfa5f09e52b.setIcon(icon_95676faa93baa877d5b5ec8fdebcf3e0);
        
    
        var popup_09698ec0a35d8fe18734420ff61d2788 = L.popup({"maxWidth": 280});

        
            var i_frame_f3d0a5cc7ba9e49e890e60dee78c94a2 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+Q2FtcG9zIEVsw61zZW9zPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFBhcsOtczwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_09698ec0a35d8fe18734420ff61d2788.setContent(i_frame_f3d0a5cc7ba9e49e890e60dee78c94a2);
        

        marker_d9dc2e0dc758b99c32ef5dfa5f09e52b.bindPopup(popup_09698ec0a35d8fe18734420ff61d2788)
        ;

        
    
    
            marker_d9dc2e0dc758b99c32ef5dfa5f09e52b.bindTooltip(
                `<div>
                     Campos Elíseos
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_e100122bb5656c47702a5a2a28cc7cbb = L.marker(
                [48.8606, 2.3376],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_b84c09dae1f2ef0dd9e103fcf8c78d2e = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_e100122bb5656c47702a5a2a28cc7cbb.setIcon(icon_b84c09dae1f2ef0dd9e103fcf8c78d2e);
        
    
        var popup_3c010cb2ef3f2f95b833c0d9294d87ec = L.popup({"maxWidth": 280});

        
            var i_frame_d5a49795529688961fe67fa5833c0b53 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+TXVzZW8gZGVsIExvdXZyZTwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBQYXLDrXM8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_3c010cb2ef3f2f95b833c0d9294d87ec.setContent(i_frame_d5a49795529688961fe67fa5833c0b53);
        

        marker_e100122bb5656c47702a5a2a28cc7cbb.bindPopup(popup_3c010cb2ef3f2f95b833c0d9294d87ec)
        ;

        
    
    
            marker_e100122bb5656c47702a5a2a28cc7cbb.bindTooltip(
                `<div>
                     Museo del Louvre
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_e3480b4f19237fef5b9c37f11c766a83 = L.marker(
                [48.86, 2.3266],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_f56c9d42b4d612566d84f50529c86e0d = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_e3480b4f19237fef5b9c37f11c766a83.setIcon(icon_f56c9d42b4d612566d84f50529c86e0d);
        
    
        var popup_a0e6489f5cacbd3f237a79f5117922cf = L.popup({"maxWidth": 280});

        
            var i_frame_c27535057c559cbe37673b5da3c1a585 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+TXVzZW8gZGUgT3JzYXk8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogUGFyw61zPC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_a0e6489f5cacbd3f237a79f5117922cf.setContent(i_frame_c27535057c559cbe37673b5da3c1a585);
        

        marker_e3480b4f19237fef5b9c37f11c766a83.bindPopup(popup_a0e6489f5cacbd3f237a79f5117922cf)
        ;

        
    
    
            marker_e3480b4f19237fef5b9c37f11c766a83.bindTooltip(
                `<div>
                     Museo de Orsay
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_0ff06aa4b6ca13e173f4292ffe995b7d = L.marker(
                [48.8636, 2.3275],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_5ac0e11ae5450d85e58ed427f7a1f8c5 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_0ff06aa4b6ca13e173f4292ffe995b7d.setIcon(icon_5ac0e11ae5450d85e58ed427f7a1f8c5);
        
    
        var popup_a355389e8ee198559c4006922e79639e = L.popup({"maxWidth": 280});

        
            var i_frame_f7c3e59058ba4bf875b00c05ea1c3584 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+SmFyZMOtbiBkZSBsYXMgVHVsbGVyw61hczwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBQYXLDrXM8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_a355389e8ee198559c4006922e79639e.setContent(i_frame_f7c3e59058ba4bf875b00c05ea1c3584);
        

        marker_0ff06aa4b6ca13e173f4292ffe995b7d.bindPopup(popup_a355389e8ee198559c4006922e79639e)
        ;

        
    
    
            marker_0ff06aa4b6ca13e173f4292ffe995b7d.bindTooltip(
                `<div>
                     Jardín de las Tullerías
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_0e07698dde2fad61806982f6e7e6ea5d = L.marker(
                [48.8656, 2.3211],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_96ebe15c32fc38a2f0e4e169e38c4b44 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_0e07698dde2fad61806982f6e7e6ea5d.setIcon(icon_96ebe15c32fc38a2f0e4e169e38c4b44);
        
    
        var popup_cb2f315d7a69138ed152f7a0a61c4a85 = L.popup({"maxWidth": 280});

        
            var i_frame_20a669a212fccf16a04531e942f3e914 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UGxhemEgZGUgbGEgQ29uY29yZGlhPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFBhcsOtczwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_cb2f315d7a69138ed152f7a0a61c4a85.setContent(i_frame_20a669a212fccf16a04531e942f3e914);
        

        marker_0e07698dde2fad61806982f6e7e6ea5d.bindPopup(popup_cb2f315d7a69138ed152f7a0a61c4a85)
        ;

        
    
    
            marker_0e07698dde2fad61806982f6e7e6ea5d.bindTooltip(
                `<div>
                     Plaza de la Concordia
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_9d221d040ca84908a5060020ee2397a6 = L.marker(
                [48.8738, 2.295],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_0539b8543668b9f9524a68beebebb9ad = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_9d221d040ca84908a5060020ee2397a6.setIcon(icon_0539b8543668b9f9524a68beebebb9ad);
        
    
        var popup_dab20929e2baca421d400fd48969434c = L.popup({"maxWidth": 280});

        
            var i_frame_8b2f20a5f07c2418e90fa37fe5926013 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+QXJjbyBkZWwgVHJpdW5mbzwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBQYXLDrXM8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_dab20929e2baca421d400fd48969434c.setContent(i_frame_8b2f20a5f07c2418e90fa37fe5926013);
        

        marker_9d221d040ca84908a5060020ee2397a6.bindPopup(popup_dab20929e2baca421d400fd48969434c)
        ;

        
    
    
            marker_9d221d040ca84908a5060020ee2397a6.bindTooltip(
                `<div>
                     Arco del Triunfo
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_857bbc8eaf03cabfd2b899c882e71add = L.marker(
                [48.8584, 2.2945],
                {}
            ).addTo(marker_cluster_1c1400456e39c1d77ad60e066754cb09);
        
    
            var icon_718c68ea465e9683d54a173f8e15bcac = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "blue", "prefix": "glyphicon"}
            );
            marker_857bbc8eaf03cabfd2b899c882e71add.setIcon(icon_718c68ea465e9683d54a173f8e15bcac);
        
    
        var popup_fbf07ea3db6cf4b957e3e7bd3c34ddea = L.popup({"maxWidth": 280});

        
            var i_frame_488808b96488a058e6acb8cdc802dd96 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+VG9ycmUgRWlmZmVsPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFBhcsOtczwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_fbf07ea3db6cf4b957e3e7bd3c34ddea.setContent(i_frame_488808b96488a058e6acb8cdc802dd96);
        

        marker_857bbc8eaf03cabfd2b899c882e71add.bindPopup(popup_fbf07ea3db6cf4b957e3e7bd3c34ddea)
        ;

        
    
    
            marker_857bbc8eaf03cabfd2b899c882e71add.bindTooltip(
                `<div>
                     Torre Eiffel
                 </div>`,
                {"sticky": true}
            );
        
    
            var feature_group_afc6c38732c55422f2cfc41076f6d4dc = L.featureGroup(
                {}
            ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
    
            var marker_86aba897191338fcd10dc0b2e05a058f = L.marker(
                [52.52, 13.405],
                {}
            ).addTo(feature_group_afc6c38732c55422f2cfc41076f6d4dc);
        
    
            var icon_b1114901ba022f322cc0b8a80ec8ab14 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "info-sign", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_86aba897191338fcd10dc0b2e05a058f.setIcon(icon_b1114901ba022f322cc0b8a80ec8ab14);
        
    
        var popup_a9913cff7dbb1f679616fc909ced5bcd = L.popup({"maxWidth": 320});

        
            var i_frame_9fb91815ec3a8b2d0d77a92af8ad6ffa = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgIDxkaXYgc3R5bGU9J2ZvbnQtZmFtaWx5OiBBcmlhbCwgc2Fucy1zZXJpZjsgd2lkdGg6IDI2MHB4Jz4KICAgICAgICA8aDQgc3R5bGU9J21hcmdpbjowIDAgNnB4IDAnPjMuIEJlcmzDrW48L2g0PgogICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+PGI+RXN0YW5jaWE6PC9iPiAyMeKAkzI0IG9jdDwvcD4KICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPjxiPkxsZWdhZGE6PC9iPiAyMSBvY3QsIDExOjIwPC9wPgogICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+PGI+U2FsaWRhOjwvYj4gMjQgb2N0LCAxMDoyMDwvcD4KICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjZweCAwIDAgMCc+VG9jYSBsb3MgbWFyY2Fkb3JlcyBjZXJjYW5vcyBwYXJhIHZlciBsb3MgcHVudG9zIGRlIGludGVyw6lzLjwvcD4KICAgIDwvZGl2PgogICAg" width="300" style="border:none !important;" height="160"></iframe>`)[0];
            popup_a9913cff7dbb1f679616fc909ced5bcd.setContent(i_frame_9fb91815ec3a8b2d0d77a92af8ad6ffa);
        

        marker_86aba897191338fcd10dc0b2e05a058f.bindPopup(popup_a9913cff7dbb1f679616fc909ced5bcd)
        ;

        
    
    
            marker_86aba897191338fcd10dc0b2e05a058f.bindTooltip(
                `<div>
                     3. Berlín (resumen)
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_cluster_140c4acdc48ecd95c577f6faf5918db7 = L.markerClusterGroup(
                {}
            );
            feature_group_afc6c38732c55422f2cfc41076f6d4dc.addLayer(marker_cluster_140c4acdc48ecd95c577f6faf5918db7);
        
    
            var marker_5accc1a90f5aaa415bdb42ecdcd53395 = L.marker(
                [52.5163, 13.3777],
                {}
            ).addTo(marker_cluster_140c4acdc48ecd95c577f6faf5918db7);
        
    
            var icon_894c113f422c7f53adc38c8894a4bae2 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_5accc1a90f5aaa415bdb42ecdcd53395.setIcon(icon_894c113f422c7f53adc38c8894a4bae2);
        
    
        var popup_ed884954821bb92634b789b44c12cb46 = L.popup({"maxWidth": 280});

        
            var i_frame_8d9bb667bdfed29ca71ac6ee73e2af24 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UHVlcnRhIGRlIEJyYW5kZWJ1cmdvPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IEJlcmzDrW48L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_ed884954821bb92634b789b44c12cb46.setContent(i_frame_8d9bb667bdfed29ca71ac6ee73e2af24);
        

        marker_5accc1a90f5aaa415bdb42ecdcd53395.bindPopup(popup_ed884954821bb92634b789b44c12cb46)
        ;

        
    
    
            marker_5accc1a90f5aaa415bdb42ecdcd53395.bindTooltip(
                `<div>
                     Puerta de Brandeburgo
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_848617e53d7eaae50a1f94a572afb9d1 = L.marker(
                [52.5186, 13.3762],
                {}
            ).addTo(marker_cluster_140c4acdc48ecd95c577f6faf5918db7);
        
    
            var icon_b08bad7a07974b8f2474add075de1a7d = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_848617e53d7eaae50a1f94a572afb9d1.setIcon(icon_b08bad7a07974b8f2474add075de1a7d);
        
    
        var popup_e8008b708068305215641ab30c007a4f = L.popup({"maxWidth": 280});

        
            var i_frame_c6b70ed71dd13590c1a0b0648853a220 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UmVpY2hzdGFnPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IEJlcmzDrW48L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_e8008b708068305215641ab30c007a4f.setContent(i_frame_c6b70ed71dd13590c1a0b0648853a220);
        

        marker_848617e53d7eaae50a1f94a572afb9d1.bindPopup(popup_e8008b708068305215641ab30c007a4f)
        ;

        
    
    
            marker_848617e53d7eaae50a1f94a572afb9d1.bindTooltip(
                `<div>
                     Reichstag
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_d81152a837c8d75a9624bc5a81816b0d = L.marker(
                [52.5145, 13.3781],
                {}
            ).addTo(marker_cluster_140c4acdc48ecd95c577f6faf5918db7);
        
    
            var icon_6841b5d7868d3bfcc799d82c0df9ccd2 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_d81152a837c8d75a9624bc5a81816b0d.setIcon(icon_6841b5d7868d3bfcc799d82c0df9ccd2);
        
    
        var popup_e9be90c9ae5ea6af634dba70cee763e7 = L.popup({"maxWidth": 280});

        
            var i_frame_de14a24019c80172f744cfa6a143ae6a = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+TWVtb3JpYWwgYSBsb3MganVkw61vcyBhc2VzaW5hZG9zIGRlIEV1cm9wYTwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBCZXJsw61uPC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_e9be90c9ae5ea6af634dba70cee763e7.setContent(i_frame_de14a24019c80172f744cfa6a143ae6a);
        

        marker_d81152a837c8d75a9624bc5a81816b0d.bindPopup(popup_e9be90c9ae5ea6af634dba70cee763e7)
        ;

        
    
    
            marker_d81152a837c8d75a9624bc5a81816b0d.bindTooltip(
                `<div>
                     Memorial a los judíos asesinados de Europa
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_305a86f4356fa4bc735df55462a04c8a = L.marker(
                [52.5167, 13.3899],
                {}
            ).addTo(marker_cluster_140c4acdc48ecd95c577f6faf5918db7);
        
    
            var icon_3ee07d1a9498e2c5bf326b6ba34ee81b = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_305a86f4356fa4bc735df55462a04c8a.setIcon(icon_3ee07d1a9498e2c5bf326b6ba34ee81b);
        
    
        var popup_e5a4696b598c786da0c2b8be8acdc7a3 = L.popup({"maxWidth": 280});

        
            var i_frame_d9f21f64cb9f6755c8c466ddf8e12c69 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+VW50ZXIgZGVuIExpbmRlbiAoYXZlbmlkYSk8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogQmVybMOtbjwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_e5a4696b598c786da0c2b8be8acdc7a3.setContent(i_frame_d9f21f64cb9f6755c8c466ddf8e12c69);
        

        marker_305a86f4356fa4bc735df55462a04c8a.bindPopup(popup_e5a4696b598c786da0c2b8be8acdc7a3)
        ;

        
    
    
            marker_305a86f4356fa4bc735df55462a04c8a.bindTooltip(
                `<div>
                     Unter den Linden (avenida)
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_42ff3c142959fe2e2b1a437c6b612b56 = L.marker(
                [52.5219, 13.4132],
                {}
            ).addTo(marker_cluster_140c4acdc48ecd95c577f6faf5918db7);
        
    
            var icon_a9570f86b1459493c2e205ff83528a6a = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_42ff3c142959fe2e2b1a437c6b612b56.setIcon(icon_a9570f86b1459493c2e205ff83528a6a);
        
    
        var popup_23a452ed2076d9abb18dddc9932fb6f6 = L.popup({"maxWidth": 280});

        
            var i_frame_daf2df3a6e1bf1d396b22982cdbfd5cf = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+QWxleGFuZGVycGxhdHo8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogQmVybMOtbjwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_23a452ed2076d9abb18dddc9932fb6f6.setContent(i_frame_daf2df3a6e1bf1d396b22982cdbfd5cf);
        

        marker_42ff3c142959fe2e2b1a437c6b612b56.bindPopup(popup_23a452ed2076d9abb18dddc9932fb6f6)
        ;

        
    
    
            marker_42ff3c142959fe2e2b1a437c6b612b56.bindTooltip(
                `<div>
                     Alexanderplatz
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_c1a51f3b1ec7ad1add7cbd721b547e10 = L.marker(
                [52.5208, 13.4094],
                {}
            ).addTo(marker_cluster_140c4acdc48ecd95c577f6faf5918db7);
        
    
            var icon_a3298574f981c497bd69737e418dca67 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_c1a51f3b1ec7ad1add7cbd721b547e10.setIcon(icon_a3298574f981c497bd69737e418dca67);
        
    
        var popup_80d8600a3d7dcef5631053a6ac60e28a = L.popup({"maxWidth": 280});

        
            var i_frame_d13907ba33de0069e185db9c8df155f4 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+VG9ycmUgZGUgVFYgKEZlcm5zZWh0dXJtKTwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBCZXJsw61uPC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_80d8600a3d7dcef5631053a6ac60e28a.setContent(i_frame_d13907ba33de0069e185db9c8df155f4);
        

        marker_c1a51f3b1ec7ad1add7cbd721b547e10.bindPopup(popup_80d8600a3d7dcef5631053a6ac60e28a)
        ;

        
    
    
            marker_c1a51f3b1ec7ad1add7cbd721b547e10.bindTooltip(
                `<div>
                     Torre de TV (Fernsehturm)
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_2613c3ef30fa6c3dae83ea31c3179766 = L.marker(
                [52.5169, 13.401],
                {}
            ).addTo(marker_cluster_140c4acdc48ecd95c577f6faf5918db7);
        
    
            var icon_f226f8fca3ff609d747e8699d3cb0191 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_2613c3ef30fa6c3dae83ea31c3179766.setIcon(icon_f226f8fca3ff609d747e8699d3cb0191);
        
    
        var popup_cc12ed6a0aa9f90d7afef0bdef64fc5a = L.popup({"maxWidth": 280});

        
            var i_frame_7b8424bca7b5e5c062bb249a27ebef4a = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+SXNsYSBkZSBsb3MgTXVzZW9zPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IEJlcmzDrW48L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_cc12ed6a0aa9f90d7afef0bdef64fc5a.setContent(i_frame_7b8424bca7b5e5c062bb249a27ebef4a);
        

        marker_2613c3ef30fa6c3dae83ea31c3179766.bindPopup(popup_cc12ed6a0aa9f90d7afef0bdef64fc5a)
        ;

        
    
    
            marker_2613c3ef30fa6c3dae83ea31c3179766.bindTooltip(
                `<div>
                     Isla de los Museos
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_b187336f68c96e176ae2889f96dda501 = L.marker(
                [52.5192, 13.401],
                {}
            ).addTo(marker_cluster_140c4acdc48ecd95c577f6faf5918db7);
        
    
            var icon_1fdf1cca3203a0edec589d6c7c0b94ab = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_b187336f68c96e176ae2889f96dda501.setIcon(icon_1fdf1cca3203a0edec589d6c7c0b94ab);
        
    
        var popup_1aaf34dbad91934859c61cee561e6418 = L.popup({"maxWidth": 280});

        
            var i_frame_b162dfa4686696fb556a0fa9246fe4dd = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+Q2F0ZWRyYWwgZGUgQmVybMOtbjwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBCZXJsw61uPC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_1aaf34dbad91934859c61cee561e6418.setContent(i_frame_b162dfa4686696fb556a0fa9246fe4dd);
        

        marker_b187336f68c96e176ae2889f96dda501.bindPopup(popup_1aaf34dbad91934859c61cee561e6418)
        ;

        
    
    
            marker_b187336f68c96e176ae2889f96dda501.bindTooltip(
                `<div>
                     Catedral de Berlín
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_ca6a90da633af23f3247abbb43dbea31 = L.marker(
                [52.5162, 13.4019],
                {}
            ).addTo(marker_cluster_140c4acdc48ecd95c577f6faf5918db7);
        
    
            var icon_01abb5257d27c0b08946521226604549 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_ca6a90da633af23f3247abbb43dbea31.setIcon(icon_01abb5257d27c0b08946521226604549);
        
    
        var popup_eb38a676af9222ebf0e06fe9dfd43235 = L.popup({"maxWidth": 280});

        
            var i_frame_2fd431ab2c665657d35eec77412d2ab3 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+SHVtYm9sZHQgRm9ydW08L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogQmVybMOtbjwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_eb38a676af9222ebf0e06fe9dfd43235.setContent(i_frame_2fd431ab2c665657d35eec77412d2ab3);
        

        marker_ca6a90da633af23f3247abbb43dbea31.bindPopup(popup_eb38a676af9222ebf0e06fe9dfd43235)
        ;

        
    
    
            marker_ca6a90da633af23f3247abbb43dbea31.bindTooltip(
                `<div>
                     Humboldt Forum
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_e45eb5a5851e5237a3d7c74b1a55b0b1 = L.marker(
                [52.5231, 13.4021],
                {}
            ).addTo(marker_cluster_140c4acdc48ecd95c577f6faf5918db7);
        
    
            var icon_445081d0d15caa0197f3cfcb25786dd4 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_e45eb5a5851e5237a3d7c74b1a55b0b1.setIcon(icon_445081d0d15caa0197f3cfcb25786dd4);
        
    
        var popup_da4de43763fd4107a1945f4de63a043f = L.popup({"maxWidth": 280});

        
            var i_frame_0582f54f3976124d4278a139ec2c6ae8 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+SGFja2VzY2hlciBNYXJrdDwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBCZXJsw61uPC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_da4de43763fd4107a1945f4de63a043f.setContent(i_frame_0582f54f3976124d4278a139ec2c6ae8);
        

        marker_e45eb5a5851e5237a3d7c74b1a55b0b1.bindPopup(popup_da4de43763fd4107a1945f4de63a043f)
        ;

        
    
    
            marker_e45eb5a5851e5237a3d7c74b1a55b0b1.bindTooltip(
                `<div>
                     Hackescher Markt
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_112b29213345e60a97c75741cf4bb048 = L.marker(
                [52.505, 13.4398],
                {}
            ).addTo(marker_cluster_140c4acdc48ecd95c577f6faf5918db7);
        
    
            var icon_0027da902d6fced16827dc8767af612d = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_112b29213345e60a97c75741cf4bb048.setIcon(icon_0027da902d6fced16827dc8767af612d);
        
    
        var popup_11768f4488d36f6c53d14e249eb50d0b = L.popup({"maxWidth": 280});

        
            var i_frame_cea0d7b72428c8e362b9a17dcf352060 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+RWFzdCBTaWRlIEdhbGxlcnkgKE11cm8gZGUgQmVybMOtbik8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogQmVybMOtbjwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_11768f4488d36f6c53d14e249eb50d0b.setContent(i_frame_cea0d7b72428c8e362b9a17dcf352060);
        

        marker_112b29213345e60a97c75741cf4bb048.bindPopup(popup_11768f4488d36f6c53d14e249eb50d0b)
        ;

        
    
    
            marker_112b29213345e60a97c75741cf4bb048.bindTooltip(
                `<div>
                     East Side Gallery (Muro de Berlín)
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_7906bae6713410b322015f77ec9c0cf8 = L.marker(
                [52.5027, 13.3958],
                {}
            ).addTo(marker_cluster_140c4acdc48ecd95c577f6faf5918db7);
        
    
            var icon_8777d075d7cc504e72688c6bd1dfb4f9 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_7906bae6713410b322015f77ec9c0cf8.setIcon(icon_8777d075d7cc504e72688c6bd1dfb4f9);
        
    
        var popup_8e92ac9776f3d07507260a2a6786e5bd = L.popup({"maxWidth": 280});

        
            var i_frame_b2fec4e833ae18fbac66deb0dc2ec98a = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+TXVzZW8gSnVkw61vIGRlIEJlcmzDrW48L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogQmVybMOtbjwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_8e92ac9776f3d07507260a2a6786e5bd.setContent(i_frame_b2fec4e833ae18fbac66deb0dc2ec98a);
        

        marker_7906bae6713410b322015f77ec9c0cf8.bindPopup(popup_8e92ac9776f3d07507260a2a6786e5bd)
        ;

        
    
    
            marker_7906bae6713410b322015f77ec9c0cf8.bindTooltip(
                `<div>
                     Museo Judío de Berlín
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_41731ddbc6846d83d0761266f46e149d = L.marker(
                [52.5246, 13.4049],
                {}
            ).addTo(marker_cluster_140c4acdc48ecd95c577f6faf5918db7);
        
    
            var icon_c8b8320d92982008ee0692e192190e9d = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_41731ddbc6846d83d0761266f46e149d.setIcon(icon_c8b8320d92982008ee0692e192190e9d);
        
    
        var popup_83e1643c628f16d82b2988d08a41a0be = L.popup({"maxWidth": 280});

        
            var i_frame_bccd198f3f405e088dd1ee3c56b84e8a = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+SWdsZXNpYSBkZSBTb2bDrWEgKFNvcGhpZW5raXJjaGUpPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IEJlcmzDrW48L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_83e1643c628f16d82b2988d08a41a0be.setContent(i_frame_bccd198f3f405e088dd1ee3c56b84e8a);
        

        marker_41731ddbc6846d83d0761266f46e149d.bindPopup(popup_83e1643c628f16d82b2988d08a41a0be)
        ;

        
    
    
            marker_41731ddbc6846d83d0761266f46e149d.bindTooltip(
                `<div>
                     Iglesia de Sofía (Sophienkirche)
                 </div>`,
                {"sticky": true}
            );
        
    
            var feature_group_829f2c9b811e7ecd7b6db0153c8c3e69 = L.featureGroup(
                {}
            ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
    
            var marker_85b7a5975b720b5cfac64b4ba017dccd = L.marker(
                [50.0755, 14.4378],
                {}
            ).addTo(feature_group_829f2c9b811e7ecd7b6db0153c8c3e69);
        
    
            var icon_c9993b86082c6d1b617cb8358b6841a2 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "info-sign", "iconColor": "white", "markerColor": "purple", "prefix": "glyphicon"}
            );
            marker_85b7a5975b720b5cfac64b4ba017dccd.setIcon(icon_c9993b86082c6d1b617cb8358b6841a2);
        
    
        var popup_2647a5e647a1766060ccc46903b38d38 = L.popup({"maxWidth": 320});

        
            var i_frame_0810b4b5dc25b6a002058b290ee7b516 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgIDxkaXYgc3R5bGU9J2ZvbnQtZmFtaWx5OiBBcmlhbCwgc2Fucy1zZXJpZjsgd2lkdGg6IDI2MHB4Jz4KICAgICAgICA8aDQgc3R5bGU9J21hcmdpbjowIDAgNnB4IDAnPjQuIFByYWdhPC9oND4KICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPjxiPkVzdGFuY2lhOjwvYj4gMjTigJMyNiBvY3Q8L3A+CiAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz48Yj5MbGVnYWRhOjwvYj4gMjQgb2N0LCAxNDoyMDwvcD4KICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPjxiPlNhbGlkYTo8L2I+IDI2IG9jdCwgMDc6NDI8L3A+CiAgICAgICAgPHAgc3R5bGU9J21hcmdpbjo2cHggMCAwIDAnPlRvY2EgbG9zIG1hcmNhZG9yZXMgY2VyY2Fub3MgcGFyYSB2ZXIgbG9zIHB1bnRvcyBkZSBpbnRlcsOpcy48L3A+CiAgICA8L2Rpdj4KICAgIA==" width="300" style="border:none !important;" height="160"></iframe>`)[0];
            popup_2647a5e647a1766060ccc46903b38d38.setContent(i_frame_0810b4b5dc25b6a002058b290ee7b516);
        

        marker_85b7a5975b720b5cfac64b4ba017dccd.bindPopup(popup_2647a5e647a1766060ccc46903b38d38)
        ;

        
    
    
            marker_85b7a5975b720b5cfac64b4ba017dccd.bindTooltip(
                `<div>
                     4. Praga (resumen)
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_cluster_836bd42f008b0635191240b834815782 = L.markerClusterGroup(
                {}
            );
            feature_group_829f2c9b811e7ecd7b6db0153c8c3e69.addLayer(marker_cluster_836bd42f008b0635191240b834815782);
        
    
            var marker_e76db7e38fdffee45fb74e7c6ce7d806 = L.marker(
                [50.0913, 14.401],
                {}
            ).addTo(marker_cluster_836bd42f008b0635191240b834815782);
        
    
            var icon_a7bf182b4097114a4b901dec27e97c87 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "purple", "prefix": "glyphicon"}
            );
            marker_e76db7e38fdffee45fb74e7c6ce7d806.setIcon(icon_a7bf182b4097114a4b901dec27e97c87);
        
    
        var popup_7f9ea0041fb8d077afe658f67c57fbce = L.popup({"maxWidth": 280});

        
            var i_frame_7d86c5858f9215e8de1ed9eff2f72f82 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+Q2FzdGlsbG8gZGUgUHJhZ2E8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogUHJhZ2E8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_7f9ea0041fb8d077afe658f67c57fbce.setContent(i_frame_7d86c5858f9215e8de1ed9eff2f72f82);
        

        marker_e76db7e38fdffee45fb74e7c6ce7d806.bindPopup(popup_7f9ea0041fb8d077afe658f67c57fbce)
        ;

        
    
    
            marker_e76db7e38fdffee45fb74e7c6ce7d806.bindTooltip(
                `<div>
                     Castillo de Praga
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_e666715f2832567cc49997566d182a71 = L.marker(
                [50.0879, 14.4046],
                {}
            ).addTo(marker_cluster_836bd42f008b0635191240b834815782);
        
    
            var icon_6631cc3309e4c1b24d9fb627e4a5c0c0 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "purple", "prefix": "glyphicon"}
            );
            marker_e666715f2832567cc49997566d182a71.setIcon(icon_6631cc3309e4c1b24d9fb627e4a5c0c0);
        
    
        var popup_08f9eb030983bb145f5120f61293b154 = L.popup({"maxWidth": 280});

        
            var i_frame_ff20a1b96038288c6ec49168e350d9c7 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+TWFsw6EgU3RyYW5hPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFByYWdhPC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_08f9eb030983bb145f5120f61293b154.setContent(i_frame_ff20a1b96038288c6ec49168e350d9c7);
        

        marker_e666715f2832567cc49997566d182a71.bindPopup(popup_08f9eb030983bb145f5120f61293b154)
        ;

        
    
    
            marker_e666715f2832567cc49997566d182a71.bindTooltip(
                `<div>
                     Malá Strana
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_683dd5f8c6e5c0fefbca12ce6feac944 = L.marker(
                [50.0905, 14.4191],
                {}
            ).addTo(marker_cluster_836bd42f008b0635191240b834815782);
        
    
            var icon_d7d3a523b27dc886659602f29f03f36d = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "purple", "prefix": "glyphicon"}
            );
            marker_683dd5f8c6e5c0fefbca12ce6feac944.setIcon(icon_d7d3a523b27dc886659602f29f03f36d);
        
    
        var popup_38538afef66d7d0ae4901832e308b275 = L.popup({"maxWidth": 280});

        
            var i_frame_a5d0e88f4f9854d82f4199396db98b49 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+QmFycmlvIEp1ZMOtbyAoSm9zZWZvdik8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogUHJhZ2E8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_38538afef66d7d0ae4901832e308b275.setContent(i_frame_a5d0e88f4f9854d82f4199396db98b49);
        

        marker_683dd5f8c6e5c0fefbca12ce6feac944.bindPopup(popup_38538afef66d7d0ae4901832e308b275)
        ;

        
    
    
            marker_683dd5f8c6e5c0fefbca12ce6feac944.bindTooltip(
                `<div>
                     Barrio Judío (Josefov)
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_2f5b0cad4e3f44236de9f94c5278754c = L.marker(
                [50.09, 14.4206],
                {}
            ).addTo(marker_cluster_836bd42f008b0635191240b834815782);
        
    
            var icon_71eb7979367b09c0e6bc3761304b9908 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "purple", "prefix": "glyphicon"}
            );
            marker_2f5b0cad4e3f44236de9f94c5278754c.setIcon(icon_71eb7979367b09c0e6bc3761304b9908);
        
    
        var popup_7359c484b429354668716f36f03e9fa6 = L.popup({"maxWidth": 280});

        
            var i_frame_7aeea973cbeaabd33726c258bb9a8f51 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+Q2VtZW50ZXJpbyBKdWTDrW88L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogUHJhZ2E8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_7359c484b429354668716f36f03e9fa6.setContent(i_frame_7aeea973cbeaabd33726c258bb9a8f51);
        

        marker_2f5b0cad4e3f44236de9f94c5278754c.bindPopup(popup_7359c484b429354668716f36f03e9fa6)
        ;

        
    
    
            marker_2f5b0cad4e3f44236de9f94c5278754c.bindTooltip(
                `<div>
                     Cementerio Judío
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_5cab70fc263ba15c9daf0281dbc73225 = L.marker(
                [50.087, 14.4208],
                {}
            ).addTo(marker_cluster_836bd42f008b0635191240b834815782);
        
    
            var icon_1de1817901dd185874c3f70760ce4688 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "purple", "prefix": "glyphicon"}
            );
            marker_5cab70fc263ba15c9daf0281dbc73225.setIcon(icon_1de1817901dd185874c3f70760ce4688);
        
    
        var popup_98584deb4ca643d42ef2079f62e43b3c = L.popup({"maxWidth": 280});

        
            var i_frame_419cc1374878ac440a34760615ee8a2c = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UmVsb2ogQXN0cm9uw7NtaWNvPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFByYWdhPC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_98584deb4ca643d42ef2079f62e43b3c.setContent(i_frame_419cc1374878ac440a34760615ee8a2c);
        

        marker_5cab70fc263ba15c9daf0281dbc73225.bindPopup(popup_98584deb4ca643d42ef2079f62e43b3c)
        ;

        
    
    
            marker_5cab70fc263ba15c9daf0281dbc73225.bindTooltip(
                `<div>
                     Reloj Astronómico
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_13e7349b5c3b32da6467e2426d5218a5 = L.marker(
                [50.0814, 14.4256],
                {}
            ).addTo(marker_cluster_836bd42f008b0635191240b834815782);
        
    
            var icon_33a0ff2b7309905c52a3fc276e5c1347 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "purple", "prefix": "glyphicon"}
            );
            marker_13e7349b5c3b32da6467e2426d5218a5.setIcon(icon_33a0ff2b7309905c52a3fc276e5c1347);
        
    
        var popup_8fe9b0fe6203f616125095d845224261 = L.popup({"maxWidth": 280});

        
            var i_frame_c3d896052913ededd930e118cd0b9d83 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UGxhemEgZGUgV2VuY2VzbGFvPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFByYWdhPC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_8fe9b0fe6203f616125095d845224261.setContent(i_frame_c3d896052913ededd930e118cd0b9d83);
        

        marker_13e7349b5c3b32da6467e2426d5218a5.bindPopup(popup_8fe9b0fe6203f616125095d845224261)
        ;

        
    
    
            marker_13e7349b5c3b32da6467e2426d5218a5.bindTooltip(
                `<div>
                     Plaza de Wenceslao
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_8c74cd03d8a78bd1402aa468b2607a72 = L.marker(
                [50.078, 14.427],
                {}
            ).addTo(marker_cluster_836bd42f008b0635191240b834815782);
        
    
            var icon_b247063e6b8aa78913417acca3217863 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "purple", "prefix": "glyphicon"}
            );
            marker_8c74cd03d8a78bd1402aa468b2607a72.setIcon(icon_b247063e6b8aa78913417acca3217863);
        
    
        var popup_551794b71b50af161ec421cffe887ade = L.popup({"maxWidth": 280});

        
            var i_frame_4e93973fededda3c18b2add52589540f = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+Tm92w6kgTcSbc3RvPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IFByYWdhPC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_551794b71b50af161ec421cffe887ade.setContent(i_frame_4e93973fededda3c18b2add52589540f);
        

        marker_8c74cd03d8a78bd1402aa468b2607a72.bindPopup(popup_551794b71b50af161ec421cffe887ade)
        ;

        
    
    
            marker_8c74cd03d8a78bd1402aa468b2607a72.bindTooltip(
                `<div>
                     Nové Město
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_a311b7c7606d4f0c19089279df348a46 = L.marker(
                [50.0865, 14.4114],
                {}
            ).addTo(marker_cluster_836bd42f008b0635191240b834815782);
        
    
            var icon_c4fd6808766621d823e76f291627ac59 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "purple", "prefix": "glyphicon"}
            );
            marker_a311b7c7606d4f0c19089279df348a46.setIcon(icon_c4fd6808766621d823e76f291627ac59);
        
    
        var popup_1f83f738a2d3b3d9ea3421482dbe8920 = L.popup({"maxWidth": 280});

        
            var i_frame_4b97869867aa96148d5b49b4b44bcbbe = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UHVlbnRlIGRlIENhcmxvczwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBQcmFnYTwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_1f83f738a2d3b3d9ea3421482dbe8920.setContent(i_frame_4b97869867aa96148d5b49b4b44bcbbe);
        

        marker_a311b7c7606d4f0c19089279df348a46.bindPopup(popup_1f83f738a2d3b3d9ea3421482dbe8920)
        ;

        
    
    
            marker_a311b7c7606d4f0c19089279df348a46.bindTooltip(
                `<div>
                     Puente de Carlos
                 </div>`,
                {"sticky": true}
            );
        
    
            var feature_group_445a45c0ddf412b33fba6ac8688c8516 = L.featureGroup(
                {}
            ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
    
            var marker_a4c727a07f916c12aade824421d3c4de = L.marker(
                [47.4979, 19.0402],
                {}
            ).addTo(feature_group_445a45c0ddf412b33fba6ac8688c8516);
        
    
            var icon_5db05a3b66524ed48ac8a32459374c1c = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "info-sign", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_a4c727a07f916c12aade824421d3c4de.setIcon(icon_5db05a3b66524ed48ac8a32459374c1c);
        
    
        var popup_0f5fc69628c7d180bb66a79eed22fbba = L.popup({"maxWidth": 320});

        
            var i_frame_fdcdb6c298d041ba3aced23e796e537b = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgIDxkaXYgc3R5bGU9J2ZvbnQtZmFtaWx5OiBBcmlhbCwgc2Fucy1zZXJpZjsgd2lkdGg6IDI2MHB4Jz4KICAgICAgICA8aDQgc3R5bGU9J21hcmdpbjowIDAgNnB4IDAnPjUuIEJ1ZGFwZXN0PC9oND4KICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPjxiPkVzdGFuY2lhOjwvYj4gMjbigJMyOSBvY3Q8L3A+CiAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz48Yj5MbGVnYWRhOjwvYj4gMjYgb2N0LCAxNDoyODwvcD4KICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPjxiPlNhbGlkYTo8L2I+IDI5IG9jdCwgMjM6NTUgKHZ1ZWxvIGEgQ0RNWCk8L3A+CiAgICAgICAgPHAgc3R5bGU9J21hcmdpbjo2cHggMCAwIDAnPlRvY2EgbG9zIG1hcmNhZG9yZXMgY2VyY2Fub3MgcGFyYSB2ZXIgbG9zIHB1bnRvcyBkZSBpbnRlcsOpcy48L3A+CiAgICA8L2Rpdj4KICAgIA==" width="300" style="border:none !important;" height="160"></iframe>`)[0];
            popup_0f5fc69628c7d180bb66a79eed22fbba.setContent(i_frame_fdcdb6c298d041ba3aced23e796e537b);
        

        marker_a4c727a07f916c12aade824421d3c4de.bindPopup(popup_0f5fc69628c7d180bb66a79eed22fbba)
        ;

        
    
    
            marker_a4c727a07f916c12aade824421d3c4de.bindTooltip(
                `<div>
                     5. Budapest (resumen)
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_cluster_49f37868f59bba1c8461a578b60572af = L.markerClusterGroup(
                {}
            );
            feature_group_445a45c0ddf412b33fba6ac8688c8516.addLayer(marker_cluster_49f37868f59bba1c8461a578b60572af);
        
    
            var marker_d58fc65778a765a9529eddedb1963ac1 = L.marker(
                [47.4961, 19.0399],
                {}
            ).addTo(marker_cluster_49f37868f59bba1c8461a578b60572af);
        
    
            var icon_586bea46eff0e592b344274d8aad4587 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_d58fc65778a765a9529eddedb1963ac1.setIcon(icon_586bea46eff0e592b344274d8aad4587);
        
    
        var popup_b011e25fc8177c798bf14b69f5729ab3 = L.popup({"maxWidth": 280});

        
            var i_frame_3dfc177168330a7f136a3a65cceef401 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+Q2FzdGlsbG8gZGUgQnVkYTwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBCdWRhcGVzdDwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_b011e25fc8177c798bf14b69f5729ab3.setContent(i_frame_3dfc177168330a7f136a3a65cceef401);
        

        marker_d58fc65778a765a9529eddedb1963ac1.bindPopup(popup_b011e25fc8177c798bf14b69f5729ab3)
        ;

        
    
    
            marker_d58fc65778a765a9529eddedb1963ac1.bindTooltip(
                `<div>
                     Castillo de Buda
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_3775760b3ae45e01dd79e271c80ff4c8 = L.marker(
                [47.4989, 19.0414],
                {}
            ).addTo(marker_cluster_49f37868f59bba1c8461a578b60572af);
        
    
            var icon_944cbb9b477293261fa0fee07b7fa558 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_3775760b3ae45e01dd79e271c80ff4c8.setIcon(icon_944cbb9b477293261fa0fee07b7fa558);
        
    
        var popup_719f0f3bb36549f68df9b24a414d7578 = L.popup({"maxWidth": 280});

        
            var i_frame_24c14fed24122ee5a579b2fae53a4e9a = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UHVlbnRlIGRlIGxhcyBDYWRlbmFzPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IEJ1ZGFwZXN0PC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_719f0f3bb36549f68df9b24a414d7578.setContent(i_frame_24c14fed24122ee5a579b2fae53a4e9a);
        

        marker_3775760b3ae45e01dd79e271c80ff4c8.bindPopup(popup_719f0f3bb36549f68df9b24a414d7578)
        ;

        
    
    
            marker_3775760b3ae45e01dd79e271c80ff4c8.bindTooltip(
                `<div>
                     Puente de las Cadenas
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_2e67ebcfee80f73b94ce8b039a351f79 = L.marker(
                [47.4938, 19.0503],
                {}
            ).addTo(marker_cluster_49f37868f59bba1c8461a578b60572af);
        
    
            var icon_11c9798b56672488879a9b120adec10f = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_2e67ebcfee80f73b94ce8b039a351f79.setIcon(icon_11c9798b56672488879a9b120adec10f);
        
    
        var popup_51cc896fd65afd76cb8622b69ade9c29 = L.popup({"maxWidth": 280});

        
            var i_frame_4f7cfdb959937f661e1da288a48e5942 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UHVlbnRlIGRlIElzYWJlbDwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBCdWRhcGVzdDwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_51cc896fd65afd76cb8622b69ade9c29.setContent(i_frame_4f7cfdb959937f661e1da288a48e5942);
        

        marker_2e67ebcfee80f73b94ce8b039a351f79.bindPopup(popup_51cc896fd65afd76cb8622b69ade9c29)
        ;

        
    
    
            marker_2e67ebcfee80f73b94ce8b039a351f79.bindTooltip(
                `<div>
                     Puente de Isabel
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_09014bf7cee9c4b92334162a12b7cd71 = L.marker(
                [47.4891, 19.058],
                {}
            ).addTo(marker_cluster_49f37868f59bba1c8461a578b60572af);
        
    
            var icon_c12d2d63f615cbf3929d4488d6cb2f86 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_09014bf7cee9c4b92334162a12b7cd71.setIcon(icon_c12d2d63f615cbf3929d4488d6cb2f86);
        
    
        var popup_4dad37d17c61b6971e15446a2c610cec = L.popup({"maxWidth": 280});

        
            var i_frame_d13c097087056c571bb596d7eedeb5d5 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+R3JhbiBNZXJjYWRvIENlbnRyYWw8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogQnVkYXBlc3Q8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_4dad37d17c61b6971e15446a2c610cec.setContent(i_frame_d13c097087056c571bb596d7eedeb5d5);
        

        marker_09014bf7cee9c4b92334162a12b7cd71.bindPopup(popup_4dad37d17c61b6971e15446a2c610cec)
        ;

        
    
    
            marker_09014bf7cee9c4b92334162a12b7cd71.bindTooltip(
                `<div>
                     Gran Mercado Central
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_0ad2b428b5c75fe6ee5c7211aa3dcfc0 = L.marker(
                [47.5054, 19.0665],
                {}
            ).addTo(marker_cluster_49f37868f59bba1c8461a578b60572af);
        
    
            var icon_69c4898c370870bcc70a4970ca469170 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_0ad2b428b5c75fe6ee5c7211aa3dcfc0.setIcon(icon_69c4898c370870bcc70a4970ca469170);
        
    
        var popup_419bd53416ba4e465c850a1f2fefd8fb = L.popup({"maxWidth": 280});

        
            var i_frame_db5bba9651ca0a1134d07f5c59e01b65 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+QXZlbmlkYSBBbmRyw6Fzc3kgKE9rdG9nb24pPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IEJ1ZGFwZXN0PC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_419bd53416ba4e465c850a1f2fefd8fb.setContent(i_frame_db5bba9651ca0a1134d07f5c59e01b65);
        

        marker_0ad2b428b5c75fe6ee5c7211aa3dcfc0.bindPopup(popup_419bd53416ba4e465c850a1f2fefd8fb)
        ;

        
    
    
            marker_0ad2b428b5c75fe6ee5c7211aa3dcfc0.bindTooltip(
                `<div>
                     Avenida Andrássy (Oktogon)
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_b69a0fedec8e94aec2ac67da75bea03c = L.marker(
                [47.5147, 19.0821],
                {}
            ).addTo(marker_cluster_49f37868f59bba1c8461a578b60572af);
        
    
            var icon_6fa38899ab9769c74d6deff348ae6172 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_b69a0fedec8e94aec2ac67da75bea03c.setIcon(icon_6fa38899ab9769c74d6deff348ae6172);
        
    
        var popup_89701052125b2ff5138fcb413f664b3b = L.popup({"maxWidth": 280});

        
            var i_frame_80048d168ba657c51e6847dbe6b10971 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UGFycXVlIGRlIGxhIENpdWRhZDwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBCdWRhcGVzdDwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_89701052125b2ff5138fcb413f664b3b.setContent(i_frame_80048d168ba657c51e6847dbe6b10971);
        

        marker_b69a0fedec8e94aec2ac67da75bea03c.bindPopup(popup_89701052125b2ff5138fcb413f664b3b)
        ;

        
    
    
            marker_b69a0fedec8e94aec2ac67da75bea03c.bindTooltip(
                `<div>
                     Parque de la Ciudad
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_5b0cc54bfe9bb621a01d34aa0f546d5b = L.marker(
                [47.5145, 19.0771],
                {}
            ).addTo(marker_cluster_49f37868f59bba1c8461a578b60572af);
        
    
            var icon_b6d28f83fc3b4b5cb6358712c2e3ae67 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_5b0cc54bfe9bb621a01d34aa0f546d5b.setIcon(icon_b6d28f83fc3b4b5cb6358712c2e3ae67);
        
    
        var popup_0ec4b39dd94eeffe5af83fe3e20a2b61 = L.popup({"maxWidth": 280});

        
            var i_frame_3dcc3d4472673af61f899ef32169631e = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UGxhemEgZGUgbG9zIEjDqXJvZXM8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogQnVkYXBlc3Q8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_0ec4b39dd94eeffe5af83fe3e20a2b61.setContent(i_frame_3dcc3d4472673af61f899ef32169631e);
        

        marker_5b0cc54bfe9bb621a01d34aa0f546d5b.bindPopup(popup_0ec4b39dd94eeffe5af83fe3e20a2b61)
        ;

        
    
    
            marker_5b0cc54bfe9bb621a01d34aa0f546d5b.bindTooltip(
                `<div>
                     Plaza de los Héroes
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_783a33d650c00e1a94620d0ad9a4e068 = L.marker(
                [47.5316, 19.046],
                {}
            ).addTo(marker_cluster_49f37868f59bba1c8461a578b60572af);
        
    
            var icon_0cfe559f0669de14c47db9a11a95017d = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_783a33d650c00e1a94620d0ad9a4e068.setIcon(icon_0cfe559f0669de14c47db9a11a95017d);
        
    
        var popup_b4b64490f911a3256d57c0f883ded66f = L.popup({"maxWidth": 280});

        
            var i_frame_7a96b9ce1469f433aac2dc8cb0ba67d7 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+SXNsYSBNYXJnYXJpdGE8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogQnVkYXBlc3Q8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_b4b64490f911a3256d57c0f883ded66f.setContent(i_frame_7a96b9ce1469f433aac2dc8cb0ba67d7);
        

        marker_783a33d650c00e1a94620d0ad9a4e068.bindPopup(popup_b4b64490f911a3256d57c0f883ded66f)
        ;

        
    
    
            marker_783a33d650c00e1a94620d0ad9a4e068.bindTooltip(
                `<div>
                     Isla Margarita
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_1a999b8896002b1351716775ee16ce59 = L.marker(
                [47.5076, 19.0451],
                {}
            ).addTo(marker_cluster_49f37868f59bba1c8461a578b60572af);
        
    
            var icon_b9b988862ba2efccb8811f26935d8bac = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_1a999b8896002b1351716775ee16ce59.setIcon(icon_b9b988862ba2efccb8811f26935d8bac);
        
    
        var popup_9f841eefcca39bffb9b1486f7ecb46c6 = L.popup({"maxWidth": 280});

        
            var i_frame_b70a66dc1ebac2d1fe568ae9b3ef9839 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+UGFybGFtZW50byBow7puZ2FybzwvaDQ+CiAgICAgICAgICAgIDxwIHN0eWxlPSdtYXJnaW46MCc+Q2l1ZGFkOiBCdWRhcGVzdDwvcD4KICAgICAgICA8L2Rpdj4KICAgICAgICA=" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_9f841eefcca39bffb9b1486f7ecb46c6.setContent(i_frame_b70a66dc1ebac2d1fe568ae9b3ef9839);
        

        marker_1a999b8896002b1351716775ee16ce59.bindPopup(popup_9f841eefcca39bffb9b1486f7ecb46c6)
        ;

        
    
    
            marker_1a999b8896002b1351716775ee16ce59.bindTooltip(
                `<div>
                     Parlamento húngaro
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_73b9753665184ec4dd77d02ad3c89aff = L.marker(
                [47.5009, 19.0534],
                {}
            ).addTo(marker_cluster_49f37868f59bba1c8461a578b60572af);
        
    
            var icon_bdf0ef793b0c30c131b0c8ade48401d7 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_73b9753665184ec4dd77d02ad3c89aff.setIcon(icon_bdf0ef793b0c30c131b0c8ade48401d7);
        
    
        var popup_53d230a092a32059678d539d77bb085b = L.popup({"maxWidth": 280});

        
            var i_frame_16dc3bdcf3e67ce5d8c2396da9712414 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+QmFzw61saWNhIGRlIFNhbiBFc3RlYmFuPC9oND4KICAgICAgICAgICAgPHAgc3R5bGU9J21hcmdpbjowJz5DaXVkYWQ6IEJ1ZGFwZXN0PC9wPgogICAgICAgIDwvZGl2PgogICAgICAgIA==" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_53d230a092a32059678d539d77bb085b.setContent(i_frame_16dc3bdcf3e67ce5d8c2396da9712414);
        

        marker_73b9753665184ec4dd77d02ad3c89aff.bindPopup(popup_53d230a092a32059678d539d77bb085b)
        ;

        
    
    
            marker_73b9753665184ec4dd77d02ad3c89aff.bindTooltip(
                `<div>
                     Basílica de San Esteban
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_eeb4df11621acfc6695c8d983a2cb189 = L.marker(
                [47.4978, 19.0616],
                {}
            ).addTo(marker_cluster_49f37868f59bba1c8461a578b60572af);
        
    
            var icon_e1f35aed66f161d4059204f16bb749ad = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_eeb4df11621acfc6695c8d983a2cb189.setIcon(icon_e1f35aed66f161d4059204f16bb749ad);
        
    
        var popup_e38a1be37669f607b3b1607fe4b286fd = L.popup({"maxWidth": 280});

        
            var i_frame_a5ef4dbc6559544b1a1b3147d3ea66d3 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+U3ppbXBsYSBLZXJ0IChydWluIGJhcik8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogQnVkYXBlc3Q8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_e38a1be37669f607b3b1607fe4b286fd.setContent(i_frame_a5ef4dbc6559544b1a1b3147d3ea66d3);
        

        marker_eeb4df11621acfc6695c8d983a2cb189.bindPopup(popup_e38a1be37669f607b3b1607fe4b286fd)
        ;

        
    
    
            marker_eeb4df11621acfc6695c8d983a2cb189.bindTooltip(
                `<div>
                     Szimpla Kert (ruin bar)
                 </div>`,
                {"sticky": true}
            );
        
    
            var marker_01c51ef6bf4d6cefcff40b0607aa2dbe = L.marker(
                [47.4946, 19.05],
                {}
            ).addTo(marker_cluster_49f37868f59bba1c8461a578b60572af);
        
    
            var icon_c93afd790f8012845366f222812cab76 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "ok-sign", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_01c51ef6bf4d6cefcff40b0607aa2dbe.setIcon(icon_c93afd790f8012845366f222812cab76);
        
    
        var popup_152dbe0ecd5b8ced3498e4aa7879e810 = L.popup({"maxWidth": 280});

        
            var i_frame_08f0bdd2493c3bd5c3ac214aa743a669 = $(`<iframe src="data:text/html;charset=utf-8;base64,CiAgICAKICAgICAgICA8ZGl2IHN0eWxlPSdmb250LWZhbWlseTogQXJpYWwsIHNhbnMtc2VyaWY7IHdpZHRoOiAyNDBweCc+CiAgICAgICAgICAgIDxoNCBzdHlsZT0nbWFyZ2luOjAgMCA2cHggMCc+RW1iYXJjYWRlcm8gRGFudWJpbyAoY3J1Y2Vybyk8L2g0PgogICAgICAgICAgICA8cCBzdHlsZT0nbWFyZ2luOjAnPkNpdWRhZDogQnVkYXBlc3Q8L3A+CiAgICAgICAgPC9kaXY+CiAgICAgICAg" width="260" style="border:none !important;" height="110"></iframe>`)[0];
            popup_152dbe0ecd5b8ced3498e4aa7879e810.setContent(i_frame_08f0bdd2493c3bd5c3ac214aa743a669);
        

        marker_01c51ef6bf4d6cefcff40b0607aa2dbe.bindPopup(popup_152dbe0ecd5b8ced3498e4aa7879e810)
        ;

        
    
    
            marker_01c51ef6bf4d6cefcff40b0607aa2dbe.bindTooltip(
                `<div>
                     Embarcadero Danubio (crucero)
                 </div>`,
                {"sticky": true}
            );
        
    
            ant_path_a1d77452e4e24a7e2d251810f6980a57 = L.polyline.antPath(
              [[40.4168, -3.7038], [48.8566, 2.3522]],
              {"bubblingMouseEvents": true, "color": "#d35400", "dashArray": [10, 20], "dashOffset": null, "delay": 800, "fill": false, "fillColor": "#d35400", "fillOpacity": 0.2, "fillRule": "evenodd", "hardwareAcceleration": false, "lineCap": "round", "lineJoin": "round", "noClip": false, "opacity": 0.8, "paused": false, "pulseColor": "#FFFFFF", "reverse": false, "smoothFactor": 1.0, "stroke": true, "weight": 4}
        ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
    
            var poly_line_b2eb2c2ac22c86065ec6c27508159284 = L.polyline(
                [[40.4168, -3.7038], [48.8566, 2.3522]],
                {"bubblingMouseEvents": true, "color": "#d35400", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "#d35400", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "noClip": false, "opacity": 0.0, "smoothFactor": 1.0, "stroke": true, "weight": 6}
            ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
    
            poly_line_b2eb2c2ac22c86065ec6c27508159284.bindTooltip(
                `<div>
                     ✈️ Vuelo Madrid → París • Sale 17 oct, 13:05 • Llega 17 oct, 15:05
                 </div>`,
                {"sticky": true}
            );
        
    
            ant_path_353dbec17b8cd38e302dad6df34cd65e = L.polyline.antPath(
              [[48.8566, 2.3522], [52.52, 13.405]],
              {"bubblingMouseEvents": true, "color": "#d35400", "dashArray": [10, 20], "dashOffset": null, "delay": 800, "fill": false, "fillColor": "#d35400", "fillOpacity": 0.2, "fillRule": "evenodd", "hardwareAcceleration": false, "lineCap": "round", "lineJoin": "round", "noClip": false, "opacity": 0.8, "paused": false, "pulseColor": "#FFFFFF", "reverse": false, "smoothFactor": 1.0, "stroke": true, "weight": 4}
        ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
    
            var poly_line_174c606d9d7a818bab52838b21e0b0a5 = L.polyline(
                [[48.8566, 2.3522], [52.52, 13.405]],
                {"bubblingMouseEvents": true, "color": "#d35400", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "#d35400", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "noClip": false, "opacity": 0.0, "smoothFactor": 1.0, "stroke": true, "weight": 6}
            ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
    
            poly_line_174c606d9d7a818bab52838b21e0b0a5.bindTooltip(
                `<div>
                     🚆 Tren París → Berlín • Sale 21 oct, 09:35 • Llega 21 oct, 11:20
                 </div>`,
                {"sticky": true}
            );
        
    
            ant_path_ccce2ef0b5b255bb2029344bc6d729f9 = L.polyline.antPath(
              [[52.52, 13.405], [50.0755, 14.4378]],
              {"bubblingMouseEvents": true, "color": "#d35400", "dashArray": [10, 20], "dashOffset": null, "delay": 800, "fill": false, "fillColor": "#d35400", "fillOpacity": 0.2, "fillRule": "evenodd", "hardwareAcceleration": false, "lineCap": "round", "lineJoin": "round", "noClip": false, "opacity": 0.8, "paused": false, "pulseColor": "#FFFFFF", "reverse": false, "smoothFactor": 1.0, "stroke": true, "weight": 4}
        ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
    
            var poly_line_d5e4c5c324599a63f1c5c40ab2145cb2 = L.polyline(
                [[52.52, 13.405], [50.0755, 14.4378]],
                {"bubblingMouseEvents": true, "color": "#d35400", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "#d35400", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "noClip": false, "opacity": 0.0, "smoothFactor": 1.0, "stroke": true, "weight": 6}
            ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
    
            poly_line_d5e4c5c324599a63f1c5c40ab2145cb2.bindTooltip(
                `<div>
                     🚆 Tren Berlín → Praga • Sale 24 oct, 10:20 • Llega 24 oct, 14:20
                 </div>`,
                {"sticky": true}
            );
        
    
            ant_path_8504b336723356d7b6d6be74ba62cd0a = L.polyline.antPath(
              [[50.0755, 14.4378], [47.4979, 19.0402]],
              {"bubblingMouseEvents": true, "color": "#d35400", "dashArray": [10, 20], "dashOffset": null, "delay": 800, "fill": false, "fillColor": "#d35400", "fillOpacity": 0.2, "fillRule": "evenodd", "hardwareAcceleration": false, "lineCap": "round", "lineJoin": "round", "noClip": false, "opacity": 0.8, "paused": false, "pulseColor": "#FFFFFF", "reverse": false, "smoothFactor": 1.0, "stroke": true, "weight": 4}
        ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
    
            var poly_line_836966c5a3dec5a1642d8d6a027adbdd = L.polyline(
                [[50.0755, 14.4378], [47.4979, 19.0402]],
                {"bubblingMouseEvents": true, "color": "#d35400", "dashArray": null, "dashOffset": null, "fill": false, "fillColor": "#d35400", "fillOpacity": 0.2, "fillRule": "evenodd", "lineCap": "round", "lineJoin": "round", "noClip": false, "opacity": 0.0, "smoothFactor": 1.0, "stroke": true, "weight": 6}
            ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
    
            poly_line_836966c5a3dec5a1642d8d6a027adbdd.bindTooltip(
                `<div>
                     🚆 Tren Praga → Budapest • Sale 26 oct, 07:42 • Llega 26 oct, 14:28
                 </div>`,
                {"sticky": true}
            );
        
    
            var layer_control_15cca25307f3b56b6ffd6c1386ddcfc1 = {
                base_layers : {
                    "openstreetmap" : tile_layer_852ca5e45a19036c94569da1fa9db7e1,
                },
                overlays :  {
                    "1. Madrid" : feature_group_9c4018803c0833d32cfb204e7660df45,
                    "2. Par\u00eds" : feature_group_43828e7afcbb140b68340dfa51cedb58,
                    "3. Berl\u00edn" : feature_group_afc6c38732c55422f2cfc41076f6d4dc,
                    "4. Praga" : feature_group_829f2c9b811e7ecd7b6db0153c8c3e69,
                    "5. Budapest" : feature_group_445a45c0ddf412b33fba6ac8688c8516,
                },
            };
            L.control.layers(
                layer_control_15cca25307f3b56b6ffd6c1386ddcfc1.base_layers,
                layer_control_15cca25307f3b56b6ffd6c1386ddcfc1.overlays,
                {"autoZIndex": true, "collapsed": false, "position": "topright"}
            ).addTo(map_0ed7fbc329ef96a2cc8a6e169afeb65c);
        
</script>
</html>
