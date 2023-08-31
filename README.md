# Testing - Podman Service Files and Systemd

## Things

After creating the pods and subsequent containers, the service file is to be templated out.

- [ ] Still need to ensure figure out the selinux context and permissions.

- [ ] Consideration of breaking each service execstart value in a seperate dict., question-mark?  Might allow for the options to be easily templated / understood, / updated / or other words that mean something, because words mean things.

- [ ] NGINX conf file needs to be added still, however unsure if using a module from another collection, or if using inherited configs from central base image, config, or more words / things.

- [ ] starting systemd as user stuff dan talked about confused about somethng...

### Changes and stuff

- [x] env.j2 item.settings.item
- [x] temp add podman_user, group and associated uids to defaults
- [x] checks for if user exists
- [x] converted the systemd tasks that dan has to handlers
