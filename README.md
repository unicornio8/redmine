Scripts redmine 
=======

* repoman.rb

Extend repoman script in redmine, for associate external repositories from console in specific projects. This association is util when you need use api for create projects and require add external repositories association with shell.

Ommit run the match between repository and project identifier like original script, and only associate existent repository to existent project in redmine

Build options is:
--addRepository project.identifier

Example:

ruby reposman.rb -r host.redmine -u url.repository --scm SCM --key APIKey --addRepository project.identifier -v

Requirements:
1. Run: gem install activeresource
2. Enable WS for repository management in redmine host.