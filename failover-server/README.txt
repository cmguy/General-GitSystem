This server has been setup as a EMM Git2 repository system server.

The Default directory /db/mysql is the top of the git repository. A link in /opt named
git points to the mysql directory so the git repository access is /opt/git.

User access is controlled to this repository using ssh keys maintained for the git userid.

Configuration Management Admin access is controlled via the following CADA groups:
- SEO_UNIX_Cemp_CM              (Host Group)
- SEO_Unix_Cemp_CM_Admins       (User Group)
- SEO_Unix_CEMP_CM_admin_accts  (Sudo Class)

The owner and group for /opt/mysql has been set to git:git for the above reasons.

Since the git user access is gitolite controlled ssh sessions, the /etc/issue and /etc/issue.net
files have been copied to "[filename]-orig" and updated.

For more details on the administration of this system, refer to
http://emm-git2.sys.comcast.net/.

Please contact the EM&M organization under Bev Tucker before changing any of this settings.

Regards,

Andy Wallace   (Andrew_Wallace@cable.comcast.com - 720-267-2677)
