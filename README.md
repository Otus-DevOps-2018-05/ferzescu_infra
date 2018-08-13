testapp_IP = 35.228.48.81
testapp_port = 9292 


bastion_IP = 35.234.126.62
someinternalhost_IP = 10.164.0.2 

Host bastion
 ForwardAgent yes
 User itriputen
 HostName 35.234.126.62
 IdentityFile ~/.ssh/id_rsa

Host someinternalhost
 User itriputen
 HostName 10.164.0.2
 ProxyJump bastion
