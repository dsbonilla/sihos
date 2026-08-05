# SIHOS - Módulo de Gestión de Pacientes

## Requisitos
XAMPP (Apache + MySQL + PHP 8.x). Sin dependencias externas.

## Instalación

1. Copiar la carpeta del proyecto en `htdocs` de XAMPP.
2. Iniciar Apache y MySQL.
3. En phpMyAdmin (o consola), importar en este orden:
   ```
   mysql -u root -p < database/schema.sql
   mysql -u root -p < database/seed.sql
   ```
4. Si tus credenciales de MySQL son distintas al default de XAMPP, ajustar en
   `config/database.php`:
   ```php
   private static string $host     = '127.0.0.1';
   private static string $dbName   = 'sihos_crud';
   private static string $user     = 'root';
   private static string $password = '';
   private static int    $port     = 3306;
   ```
5. Acceder a `http://localhost/sihos_crud/`

**Usuario de prueba:** `admin` / **Contraseña:** `1234567890`
