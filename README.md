The Setup
=========

This is a docker-compose file for a simple, secure torrent setup. It includes
[rTorrent] (a torrent client), [flood] (a web interface for rTorrent), [OpenVPN]
(to tunnel traffic through your ISP) and a simple iptables firewall to allow
rTorrent to only access the internet through a VPN.

To run everything, put your open vpn configuration file in `./vpn.ovpn` and the
other configuration files from this gist in a directory then go to that
directory and run

    docker-compose up

Now flood can be accessed by visiting localhost:3000.

🎉

[rTorrent]: https://github.com/rakshasa/rtorrent
[flood]: https://github.com/jfurrow/flood
[OpenVPN]: https://openvpn.net/
[simple-firewall]: https://github.com/0xcaff/docker-simple-firewall
