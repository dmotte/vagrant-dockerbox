# test

This is a usage example for the [`dmotte/dockerbox`](https://app.vagrantup.com/dmotte/boxes/dockerbox) Vagrant box.

From here on, let's assume you have put this folder in `~/dockerbox01` on your PC.

Now customize the [`Vagrantfile`](Vagrantfile); in particular, you may want to customize the `config.vm.synced_folder` section. For example:

```ruby
config.vm.synced_folder "~/git", "/home/vagrant/git"
```

This means that the `~/git` folder on your PC will be mounted to `/home/vagrant/git` inside the VM.

Then, from the `~/dockerbox01` directory, run the following command to **bring up your VM**:

```bash
vagrant up
```

Add the following **alias** to your `~/.bashrc` file (replacing the script path with the correct one for your case):

```bash
alias dockerboxssh="$HOME/dockerbox01/dockerboxssh.sh"
```

Open a new shell window. Now you can execute stuff in your VM from any directory within your `~/git` folder, using the `dockerboxssh` alias command. For example:

```bash
dockerboxssh docker ps -a
```
