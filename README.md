# ansible


This project is a Sysadmins demonstration of how Ansible and DevOps tools can be used.


Under the group_vars folder is an example for each role. Don’t edit the example_ files, copy the file and remove the "example_" from the name. The playbook examples will use the newly created file. You can edit the file to fit your environments needs.


Roles

	• Windows
		○ win_domain_controller
			§ Sets up the first domain controller in a domain.
			§ Variables: 
				□ domain_controller_hostname: 
				□ active_directory_domain_name: 
				□ domain_admin_password: 
				□ active_directory_recovery_password: 
		○ win_create_shared_folder
			§ Creates a single folder share. NTFS permissions can be set using "win_create_shared_folder_rights". Adds user/group with full rights on the share
			§ Variables: 
				□ win_create_shared_folder_path: 
				□ win_create_shared_folder_user: 
				□ win_create_shared_folder_rights: 
				□ win_create_shared_folder_type: 
				□ win_create_shared_folder_state1: 
				□ win_create_shared_folder_state2: 
				□ win_create_shared_folder_propagation: 
				□ win_create_shared_folder_name: 
				□ win_create_shared_folder_description: 
				□ win_create_shared_folder_list: 
				□ win_create_shared_folder_full: 
		○ win_joindomian
			§ Joins PC/Servers to the domain and places the device in a set OU.
			§ You will need a user account with rights to join devices to the domain. 
			§ Variables: 
				□ domain_name: 
				□ domain_user: 
				□ domain_user_password: 
				□ domain_ou: 
		
			
			
			
			
	• Ubuntu
		○ ub_unifi
			§ Installs Ubiquiti's UniFi controller.
			§ Varibles: 
				□ ub_unifi_apt_name1: 
				□ ub_unifi_apt_name2: 
				□ ub_unifi_apt_name3: 
				□ ub_unifi_mongo_key_url: 
				□ ub_unifi_unifi_key_url: 
				□ ub_unifi_mongo_repo: 
				□ ub_unifi_unifi_repo: 
				□ ub_unifi_mongo_repo_filename: 
				□ ub_unifi_unifi_repo_filename: 

https://helpfulitnotes.com
