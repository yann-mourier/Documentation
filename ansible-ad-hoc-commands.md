# Créer un utilisateur
</code>ansible localhost -m ansible.builtin.user -a "name=username password=motdepasse" -b</code>

# Supprimer un utilisateur
</code>ansible localhost -m ansible.builtin.user -a "name=username state=absent" -b</code>

# Créer un fichier contenant du texte
</code>ansible localhost -m ansible.builtin.copy -a "content=Hello World! dest=~/file.txt"</code>

# Installer apache2
</code>ansible localhost -m apt -a "name=apache2 state=present" -b</code>

# Installer curl
</code>ansible localhost -m apt -a "name=curl state=present" -b</code>

# Installer podman
</code>ansible localhost -m apt -a "name=podman state=present" -b</code>