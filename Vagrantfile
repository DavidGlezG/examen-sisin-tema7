
Vagrant.configure("2") do |config|
 
  config.vm.box = "ubuntu/xenial64"
  config.vm.hostname = "david-gonzalez-garcia"
 
  config.vm.provision "shell", inline: <<-SHELL
 
    echo "-- Insertar datos de ejemplo en la tabla 'menu' " > /home/vagrant/menu.sql
    echo "INSERT INTO gestion_restaurante.menu (idPlato, nombre, descripcion, precio, categoria) VALUES" >> /home/vagrant/menu.sql
    echo "(7, 'Revuelto de huevos', 'Revuelto de varios huevos con un poco de jamón', 11.25, 'Plato combinado')," >> /home/vagrant/menu.sql
    echo "(11, 'Pasta a la carbonara', 'Pasta de tu elección con salsa carbonara', 13.99, 'Comida italiana')," >> /home/vagrant/menu.sql
    echo "(18, 'Filete con patatas', 'Carne de primera calidad con una ración de patatas', 14.50, 'Plato combinado')," >> /home/vagrant/menu.sql
    echo "(3, 'Fabada', 'Fabada casera de la casa', 16.50, 'Comida asturiana')" >> /home/vagrant/menu.sql
 
 
  SHELL
 
end
