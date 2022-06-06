host-cluster List → 생성한 VM의 hostname을 넣어줍니다.(NCP에서 VM을 생성할 때, oidc을 넣어주어서 oidc001, 002, 003으로 생성되게 초기에 셋팅합니다.)
※ 예시
oidc001    ansible_host=192.168.0.6   ansible_connection=ssh   node_role=infra
oidc002    ansible_host=192.168.0.7   ansible_connection=ssh   node_role=infra
oidc003    ansible_host=192.168.0.8   ansible_connection=ssh   node_role=infra

member-cluster List
패스

Group List
[local] → 기본값으로 나둡니다.
install-server

[host-master] → Master 1번의 hostname을 입력합니다.
oidc001 

[host-master-cluster] → 패스
#acc-host-master2
#acc-host-master3

[host-minions] → Worker 서버 2대의 hostname을 입력합니다.
oidc002
oidc003

[host-cluster] → 전체 서버 hostname을 전부 넣어줍니다.
oidc001
oidc002
oidc003

나머지는 건드리지 않습니다.
