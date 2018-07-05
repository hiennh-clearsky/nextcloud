# nextcloud
Nextcloud architecture
         
CLIENT -- PROXY -- NEXTCLOUD 

1. Proxy: HAproxy 1.8
1.1 Terminate SSL
1.2 Send X-Forwarded-For
1.3 Reverse proxy based on request domain names
2. Nextcloud: Snap on Ubuntu 16.04
2.1 Enable trusted_proxies
2.2 Enable X-Forwarded-For
2.3 Enable auth.bruteforce.protection.enabled
3. File system: Btrfs
4. Backend block storage: CEPH Mimic
