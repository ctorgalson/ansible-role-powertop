# Ansible Role Powertop

This is a simple role that creates a service to run commands in `rc.local`.

Specifically, it runs `sudo powertop --auto-tune` at startup. Note that this could change if I find that Powertop's auto-tuning is unsuited to the hardware I'm running on, or Powertop just needs more detailed configuration.

## Role Variables


| Variable name  | Default value | Description |
|----------------|---------------|-------------|
| `powertop_command` | `powertop --auto-tune` | The powertop command to run at startup. |
| `powertop_file_name` | `rc.local` | The name of the file to create in `/etc`. |
| `powertop_service_name` | `rc-local` | `The name of the service to create.` |


## License

MIT

## Author Information

Christopher Torgalson
