configure_file(input: 'ogon-rdp-server.service.in', output: 'ogon-rdp-server.service', configuration: cdata)
configure_file(input: 'ogon-session-manager.service.in', output: 'ogon-session-manager.service', configuration: cdata)
configure_file(input: 'ogon-session-manager.init.in', output: 'ogon-session-manager.init', configuration: cdata)
configure_file(input: 'ogon-rdp-server.init.in', output: 'ogon-rdp-server.init', configuration: cdata)
configure_file(input: 'config.ini.debian.in', output: 'config.ini.debian', configuration: cdata)

if get_option('with_openh264')
	configure_file(input: 'ogon-get-openh264-codec.in', 
			output: 'ogon-get-openh264-codec', 
			configuration: cdata,
			install_dir: get_option('sbindir')
	)
endif

install_data('ogonXsession', install_dir: ogon_cfg_path)
install_data('ogon_cleanup.sh', install_dir: ogon_cfg_path)