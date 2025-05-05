## Dictionnaire de données pour le bot onboarding

| Nom de la table         | Nom de la colonne           | Type   | Précision         | exemple                                | Description                                                  |
| ----------------------- | --------------------------- | ------ | ----------------- | -------------------------------------- | ------------------------------------------------------------ |
| Guilds                  | `id_guild`                  | text   | 17-19(sflake)     | "123456789012345678"                   | Identifiant unique du serveur Discord                        |
| Guilds                  | `name`                      | text   | 2-100             | "simplon serveur hdf"                  | Nom du serrveur Discord                                      |
| Guilds                  | `member_count`              | int    | chaine numérique  | 100                                    | Nombre de membres du serveur Discord                         |
| Guilds                  | `configuration`             | object |                   | "{ welcomeChan: '123', prefix: '!' }"  | Configuration du serveur Discord                             |
| Guilds_templates        | `id_guild_template`         | text   | 17-19(sflake)     | "123456789012345678"                   | Identifiant unique du template de serveur Discord            |
| Guilds_templates        | `name`                      | text   | 2-100             | "template simplon"                     | Nom du template de serveur Discord                           |
| Members                 | `id_members`                | text   | 36(uuid)          | "550e8400-e29b-41d4-a716-446655440000" | Identifiant unique du membre Discord                         |
| Members                 | `guild_username`            | text   | 1-32              | "Jean Dupont"                          | Surnom de serveur discord du membre Discord                  |
| Members_informations    | `id_member_info`            | text   | 36(uuid)          | "550e8400-e29b-41d4-a716-446655440000" | Identifiant unique des informations du membre Discord        |
| Members_informations    | `firstname`                 | text   | 50                | "Jean"                                 | Prénom du membre Discord                                     |
| Members_informations    | `lastname`                  | text   | 50                | "Dupont"                               | Nom de famille du membre Discord                             |
| Members_informations    | `email`                     | text   | 255               | "jean.dupont@example.com"              | Adresse email du membre Discord                              |
| discord_users           | `id_discord`                | text   | 17-19(sflake)     | "123456789012345678"                   | Identifiant unique du membre Discord                         |
| discord_users           | `discord_user_name`         | text   | 2-32              | "JeanDupont" de JeanDupont#1234        | Nom d'utilisateur du membre Discord                          |
| discord_users           | `discriminator`             | text   | 4(digits)         | "1234"                                 | Discriminant du membre Discord                               |
| identification_requests | `id_identification_request` | text   | 36(uuid)          | "550e8400-e29b-41d4-a716-446655440000" | Identifiant unique de la demande d'identification            |
| identification_requests | `firstname`                 | text   | 50                | "Jean"                                 | Prénom de la personne effectuant la demande d'identification |
| identification_requests | `lastname`                  | text   | 50                | "Dupont"                               | Nom de la personne effectuant la demande d'identification    |
| identification_requests | `email`                     | text   | 255               | "jean.dupont@example.com"              | Email de la personne effectuant la demande d'identification  |
| Roles                   | `id_role`                   | text   | 17-19(sflake)     | "123456789012345678"                   | Identifiant unique du rôle Discord                           |
| Roles                   | `name`                      | text   | 50                | "cdp"                                  | Nom du rôle Discord                                          |
| Roles                   | `member_count`              | int    | chaine numérique  | 10                                     | Nombre de membres avec ce rôle Discord                       |
| Roles                   | `role_position`             | int    | chaine numérique  | 1                                      | Position au sein de ce rôle Discord                          |
| Roles                   | `hoist`                     | bool   |                   | true                                   | Si dans une section séparée de la liste des utilisateurs     |
| Roles                   | `color`                     | text   | 7                 | "#FF0000"                              | Couleur hexadecimale du rôle Discord                         |
| Campuses                | `id_campus`                 | text   | 17-19(sflake)     | "123456789012345678"                   | Identifiant unique du campus                                 |
| Campuses                | `name`                      | text   | 50                | "Valenciennes"                         | Nom du campus                                                |
| Promotions              | `id_promotion`              | text   | 17-19(sflake)     | "123456789012345678"                   | Identifiant unique de la promotion                           |
| Promotions              | `name`                      | text   | 100               | "CDA-vals-p4"                          | nom de la promotion                                          |
| Promotions              | `is_active`                 | bool   |                   | true                                   | Si la promotion est active                                   |
| Promotions              | `start_date`                | date   |                   | "2024-01-01T00:00:00.000Z"             | date de début de la promotion                                |
| Promotions              | `end_date`                  | date   |                   | "2025-12-31T23:59:59.999Z"             | date de fin de la promotion                                  |
| Courses                 | `id_courses`                | text   | 17-19(sflake)     | "123456789012345678"                   | identifiant unique de la formation                           |
| Courses                 | `name`                      | text   | 3-50              | "CDA"                                  | nom de la formation                                          |
| Courses                 | `is_certified`              | bool   |                   | true                                   | Si la formation est certifiante                              |
| Channels                | `id_channel`                | text   | 17-19(sflake)     | "123456789012345678"                   | identifiant unique du channel                                |
| Channels                | `name`                      | text   | 50                | "général"                              | nom du channel                                               |
| Channels                | `type`                      | text   | (enum text/voice) | "text"                                 | Type de channel (texte ou vocal)                             |
| Channels                | `channel_position`          | int    | chaine numérique  | 1                                      | Positionnement du channel                                    |
| Categories              | `id_category`               | text   | 17-19(sflake)     | "123456789012345678"                   | identifiant unique de la catégorie                           |
| Categories              | `name`                      | text   | 50                | "stock"                                | nom de la catégorie                                          |
| Categories              | `category_position`         | int    | chaine numérique  | 0                                      | positionnement de la catégorie dans le serveur               |
|                         |                             |        |                   |                                        |                                                              |
