
### master isolation ( yes / no )
master_isolation: "yes" \
 → Master에 Pod를 배포할 것인지 선택하는 옵션입니다. Master의 부하를 줄이기 위해 yes로 설정합니다.

 
### master_host_name: "oidc001" 			
 → Master 1번의 hostname을 입력합니다.
master_ip: 192.168.0.6 					
 → Master 1번의 IP를 입력합니다.
 
### nfs_setup ( internal / external )
nfs_setup: "external" 					
 → 외부 NAS를 사용하기에 external로 변경합니다.
 
### nfs_server_ip: 169.254.84.49 			
 → NCP에서 생성한 NAS IP를 넣습니다.
 
### accordion_nfs_path: "/n2863303_oidc" 	
 → NCP에서 알려준 NAS 경로를 넣습니다.


### nfs_version ( v3 / v4 )
nfs_version: "v4"\
 → NCP는 NFS버전을 v4로 사용합니다. v4로 변경합니다.


### accordion_registry_option ( local / external )
base_registry_option: "local"\
base_registry_address: 192.168.0.6	
 → Master 1번의 IP를 입력합니다.\
base_registry_port: 5000\
base_registry_id: accregistry\
base_registry_passwd: accordionadmin

### registry_option ( registry / harbor)
user_registry_option: "registry"\
user_registry_address: 192.168.0.6	
 → Master 1번의 IP를 입력합니다.\
user_registry_port: 30001

### Calico Mode (IPIP & vxlan)
calico_backend: "vxlan"\
 → NCP는 IPIP 통신이 되지 않는 이슈가 있기 때문에 vxlan으로 변경합니다.


### containers_storage_runroot: /oidc/var/run/containers 
 → 새롭게 추가한 스토리지로 경로를 변경합니다.
 
### containers_storage_volume: /oidc/var/lib/containers  
 → 새롭게 추가한 스토리지로 경로를 변경합니다.


### docker_rpm_dir: /oidc/tmp 				
 → 새롭게 추가한 스토리지로 경로를 변경합니다.
 
나머지는 건드리지 않습니다.
