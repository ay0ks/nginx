## nginx

### Directory structure
 - `certs.d`: You should put your certifcates and keys here.
 - `conf.d`: Anything that extends `nginx.conf` and is included by it should be placed here.
 - `conf.extra.d`: Anything that is used either by vhosts in `conf.sites.d` or upstreams in `conf.upstreams.d` or `nginx.conf`.
 - `conf.sites.d`: Virtual hosts go here.
 - `conf.upstreams.d`: Upstream configurations go here.
 - `conf.modules.d`: Symbolic link to `/usr/lib/nginx/modules`, nginx modules should put their files here (you can symlink this to `modules` to avoid errors when installing.)
 - `logs.d`: Nginx logs go here, you also should your vhost or upstream configurations to store logs here (you can link this to `/var/log` if you want.)

```bash
sudo su
cd /etc
git clone https://github.com/ay0ks/nginx.git
cd nginx
```
```bash
systemctl restart nginx
```
