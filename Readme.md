#1.свободные подсети

          192.168.0.16/28
          192.168.0.48/28
          192.168.0.128/25

#2.количество узлов в каждой подсети, включая свободные

          central = 244 hosts
          office1 = 248 hosts
          office2 = 250 hosts, 

#3.broadcast адрес для каждой подсети

          192.168.0.0/16 (255.255.0.0):
              65534 hosts
              192.168.255.255 = BROADCAST

#

              Cеть 192.168.0.0/22:
          	hosts 1022
          	192.168.3.255 = BROADCAST

#

          	Сеть central - 192.168.0.0/24:
                      192.168.0.0/28 - directors
          	        14 hosts 
                          192.168.0.15 = BROADCAST
                      >------------------------------
                      192.168.0.16/28 - FREE SUBNET
                          14 hosts
                      192.168.0.31 = BROADCAST
                      ------------------------------<
                      192.168.0.32/28 - office hardware
                          14 hosts 
                      192.168.0.47 = BROADCAST
          	    >------------------------------
          	    192.168.0.48/28 - FREE SUBNET
          		14 hosts
          	    192.168.0.63 = BROADCAST
          	    ------------------------------<
                      192.168.0.64/26 - wifi
                          62 hosts
                      192.168.0.127 = BROADCAST
          	    >------------------------------
                      192.168.0.128/25 - FREE SUBNET
                          126 hosts
                      192.168.0.255 = BROADCAST
                      ------------------------------<

#

          	Сеть office2 - 192.168.1.0/24:
                      192.168.1.0/25 - dev
                          126 hosts 
                      	192.168.1.127 = BROADCAST
                      192.168.1.128/26 - test servers
                          62 hosts 
                      192.168.1.191 = BROADCAST
                      192.168.1.192/26 - office hardware
                          62 hosts 
                      192.168.1.255 = BROADCAST

#

                  Сеть office1 - 192.168.2.0/24:
                      192.168.2.0/26 - dev
          		62 hosts
          		192.168.2.63 = BROADCAST
                      192.168.2.64/26 - test servers
          		62 hosts
          		192.168.2.127 = BROADCAST
                      192.168.2.128/26 - managers
          		62 hosts
          		192.168.2.191 = BROADCAST
                      192.168.2.192/26 - office hardware
          		62 hosts
          		192.168.2.255 = BROADCAST

#
	
                  Сеть FREE - 192.168.3.0/24
          		254 hosts
          		192.168.3.255 = BROADCAST

#
	
                  Сеть FREE2 - 192.168.4.0/22
                       1022 hosts
                       192.168.7.255 = BROADCAST
	  
#
    
                 Сеть FREE - 192.168.252.0/22
                	1022 hosts
                      192.168.255.255 = BROADCAST



