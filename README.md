# CISCO_SWITCH-2960_CLI-Command-line-interface-configuration

Fa0/3                        connected    trunk      auto    auto  10/100BaseTX
Fa0/4                        notconnect   1          auto    auto  10/100BaseTX
Fa0/5                        notconnect   1          auto    auto  10/100BaseTX
Fa0/6                        notconnect   1          auto    auto  10/100BaseTX
Fa0/7                        notconnect   1          auto    auto  10/100BaseTX
Fa0/8                        notconnect   1          auto    auto  10/100BaseTX
Fa0/9                        notconnect   1          auto    auto  10/100BaseTX
Fa0/10                       notconnect   1          auto    auto  10/100BaseTX
Fa0/11                       notconnect   1          auto    auto  10/100BaseTX
Fa0/12                       notconnect   1          auto    auto  10/100BaseTX
Fa0/13                       notconnect   1          auto    auto  10/100BaseTX
Fa0/14                       notconnect   1          auto    auto  10/100BaseTX
Fa0/15                       notconnect   1          auto    auto  10/100BaseTX
Fa0/16                       notconnect   1          auto    auto  10/100BaseTX
Fa0/17                       notconnect   1          auto    auto  10/100BaseTX
Fa0/18                       notconnect   1          auto    auto  10/100BaseTX
Fa0/19                       notconnect   1          auto    auto  10/100BaseTX
Fa0/20                       notconnect   1          auto    auto  10/100BaseTX
Fa0/21                       notconnect   1          auto    auto  10/100BaseTX

Switch(config-if)#
Switch(config-if)#exit
Switch(config)#interface FastEthernet0/3
Switch(config-if)#
Switch(config-if)#exit
Switch(config)#interface FastEthernet0/1
Switch(config-if)#
Switch(config-if)#exit
Switch(config)#interface FastEthernet0/1
Switch(config-if)#description ## to pc0 ##
Switch(config-if)#exit
Switch(config)#do show interface status
Port      Name               Status       Vlan       Duplex  Speed Type
Fa0/1     ## to pc0 ##       notconnect   1          a-full  a-100 10/100BaseTX
Fa0/2                        connected    1          auto    auto  10/100BaseTX
Fa0/3                        connected    trunk      auto    auto  10/100BaseTX
Fa0/4                        notconnect   1          auto    auto  10/100BaseTX
Fa0/5                        notconnect   1          auto    auto  10/100BaseTX
Fa0/6                        notconnect   1          auto    auto  10/100BaseTX
Fa0/7                        notconnect   1          auto    auto  10/100BaseTX
Fa0/8                        notconnect   1          auto    auto  10/100BaseTX
Fa0/9                        notconnect   1          auto    auto  10/100BaseTX
Fa0/10                       notconnect   1          auto    auto  10/100BaseTX
Fa0/11                       notconnect   1          auto    auto  10/100BaseTX
Fa0/12                       notconnect   1          auto    auto  10/100BaseTX
Fa0/13                       notconnect   1          auto    auto  10/100BaseTX
Fa0/14                       notconnect   1          auto    auto  10/100BaseTX
Fa0/15                       notconnect   1          auto    auto  10/100BaseTX
Fa0/16                       notconnect   1          auto    auto  10/100BaseTX
Fa0/17                       notconnect   1          auto    auto  10/100BaseTX
Fa0/18                       notconnect   1          auto    auto  10/100BaseTX
Fa0/19                       notconnect   1          auto    auto  10/100BaseTX
Fa0/20                       notconnect   1          auto    auto  10/100BaseTX
Fa0/21                       notconnect   1          auto    auto  10/100BaseTX
Fa0/22                       notconnect   1          auto    auto  10/100BaseTX
Fa0/23                       notconnect   1          auto    auto  10/100BaseTX
Fa0/24                       notconnect   1          auto    auto  10/100BaseTX
Gig0/1                       connected    1          auto    auto  10/100BaseTX
Gig0/2                       notconnect   1          auto    auto  10/100BaseTX

Switch(config)#
Switch(config)#interface f0/1
Switch(config-if)#speed auto
Switch(config-if)#duplex auto
Switch(config-if)#
%LINK-5-CHANGED: Interface FastEthernet0/1, changed state to up

%LINEPROTO-5-UPDOWN: Line protocol on Interface FastEthernet0/1, changed state to up

Switch(config-if)#exit
Switch(config)#do show interface status
Port      Name               Status       Vlan       Duplex  Speed Type
Fa0/1     ## to pc0 ##       connected    1          auto    auto  10/100BaseTX
Fa0/2                        connected    1          auto    auto  10/100BaseTX
Fa0/3                        connected    trunk      auto    auto  10/100BaseTX
Fa0/4                        notconnect   1          auto    auto  10/100BaseTX
Fa0/5                        notconnect   1          auto    auto  10/100BaseTX
Fa0/6                        notconnect   1          auto    auto  10/100BaseTX
Fa0/7                        notconnect   1          auto    auto  10/100BaseTX
Fa0/8                        notconnect   1          auto    auto  10/100BaseTX
Fa0/9                        notconnect   1          auto    auto  10/100BaseTX
Fa0/10                       notconnect   1          auto    auto  10/100BaseTX
Fa0/11                       notconnect   1          auto    auto  10/100BaseTX
Fa0/12                       notconnect   1          auto    auto  10/100BaseTX
Fa0/13                       notconnect   1          auto    auto  10/100BaseTX
Fa0/14                       notconnect   1          auto    auto  10/100BaseTX
Fa0/15                       notconnect   1          auto    auto  10/100BaseTX
Fa0/16                       notconnect   1          auto    auto  10/100BaseTX
Fa0/17                       notconnect   1          auto    auto  10/100BaseTX
Fa0/18                       notconnect   1          auto    auto  10/100BaseTX
Fa0/19                       notconnect   1          auto    auto  10/100BaseTX
Fa0/20                       notconnect   1          auto    auto  10/100BaseTX
Fa0/21                       notconnect   1          auto    auto  10/100BaseTX
Fa0/22                       notconnect   1          auto    auto  10/100BaseTX
Fa0/23                       notconnect   1          auto    auto  10/100BaseTX
Fa0/24                       notconnect   1          auto    auto  10/100BaseTX
Gig0/1                       connected    1          auto    auto  10/100BaseTX
Gig0/2                       notconnect   1          auto    auto  10/100BaseTX

Switch(config)#interface range f0/4 - f0/24
Switch(config-if-range)#description ## not in use ##
Switch(config-if-range)#exit
Switch(config)#do show interface status
Port      Name               Status       Vlan       Duplex  Speed Type
Fa0/1     ## to pc0 ##       connected    1          auto    auto  10/100BaseTX
Fa0/2                        connected    1          auto    auto  10/100BaseTX
Fa0/3                        connected    trunk      auto    auto  10/100BaseTX
Fa0/4     ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/5     ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/6     ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/7     ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/8     ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/9     ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/10    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/11    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/12    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/13    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/14    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/15    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/16    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/17    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/18    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/19    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/20    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/21    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/22    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/23    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Fa0/24    ## not in use ##   notconnect   1          auto    auto  10/100BaseTX
Gig0/1                       connected    1          auto    auto  10/100BaseTX
Gig0/2                       notconnect   1          auto    auto  10/100BaseTX

Switch(config)#interface range f0/4 - f0/24
Switch(config-if-range)#shutdown

%LINK-5-CHANGED: Interface FastEthernet0/4, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/5, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/6, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/7, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/8, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/9, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/10, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/11, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/12, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/13, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/14, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/15, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/16, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/17, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/18, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/19, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/20, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/21, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/22, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/23, changed state to administratively down

%LINK-5-CHANGED: Interface FastEthernet0/24, changed state to administratively down
Switch(config-if-range)#exit
Switch(config)#do show interface status
Port      Name               Status       Vlan       Duplex  Speed Type
Fa0/1     ## to pc0 ##       connected    1          auto    auto  10/100BaseTX
Fa0/2                        connected    1          auto    auto  10/100BaseTX
Fa0/3                        connected    trunk      auto    auto  10/100BaseTX
Fa0/4     ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/5     ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/6     ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/7     ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/8     ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/9     ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/10    ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/11    ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/12    ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/13    ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/14    ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/15    ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/16    ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/17    ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/18    ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/19    ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/20    ## not in use ##   disabled 1          auto    auto  10/100BaseTX
Fa0/21    ## not in use ##   disabled 1          auto    auto  10/100BaseTX
