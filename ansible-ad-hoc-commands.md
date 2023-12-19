# Créer un utilisateur
`ansible localhost -m ansible.builtin.user -a "name=username password=motdepasse" -b`

# Supprimer un utilisateur
`ansible localhost -m ansible.builtin.user -a "name=username state=absent" -b`

# Créer un fichier contenant du texte
`ansible localhost -m ansible.builtin.copy -a "content=Hello World! dest=~/file.txt"`

# Installer apache2
`ansible localhost -m apt -a "name=apache2 state=present" -b`

# Installer curl
`ansible localhost -m apt -a "name=curl state=present" -b`

# Installer podman
`ansible localhost -m apt -a "name=podman state=present" -b`