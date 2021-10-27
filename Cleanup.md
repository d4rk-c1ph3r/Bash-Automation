
# Remove cache and additional zip files
ln -sf /dev/null /root/.bash_history
ln -sf /dev/null /home/$USER/.bash_history

rm -rf /root/build.sh
rm -rf /root/.cache
rm -rf /root/app*
rm -rf /home/$USER/.sudo_as_admin_successful
rm -rf /home/$USER/.cache
find /var/log -type f -exec sh -c "cat /dev/null > {}" \;
