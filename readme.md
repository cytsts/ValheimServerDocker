* atualizar em breve

version: "3"
services:
  valheim:
    image: mbround18/valheim:latest
    ports:
      - "2456:2456/udp"
      - "2457:2457/udp"
      - "2458:2458/udp"
    environment:
      TYPE: ValheimPlus
      PORT: 2456
      NAME: "Created With Valheim Docker"
      WORLD: "Dedicated"     
      TZ: "America/Chicago"
      PUBLIC: 0
      AUTO_UPDATE: 1
      AUTO_UPDATE_SCHEDULE: "0 1 * * *"
      AUTO_BACKUP: 1
      AUTO_BACKUP_SCHEDULE: "*/15 * * * *"
      AUTO_BACKUP_REMOVE_OLD: 1
      AUTO_BACKUP_DAYS_TO_LIVE: 3
      AUTO_BACKUP_ON_UPDATE: 1
      AUTO_BACKUP_ON_SHUTDOWN: 1
      #WEBHOOK_URL: "https://discord.com/api/webhooks/IM_A_SNOWFLAKE/AND_I_AM_A_SECRET"
      #WEBHOOK_INCLUDE_PUBLIC_IP: 1
      UPDATE_ON_STARTUP: 0
      MODS :   https://cdn.thunderstore.io/live/repository/packages/denikson-BepInExPack_Valheim-5.4.1900.zip
              ,https://cdn.thunderstore.io/live/repository/packages/ValheimModding-Jotunn-2.6.2.zip
              ,https://cdn.thunderstore.io/live/repository/packages/ValheimModding-HookGenPatcher-0.0.3.zip
              ,https://cdn.thunderstore.io/live/repository/packages/MathiasDecrock-PlanBuild-0.9.5.zip
              ,https://cdn.thunderstore.io/live/repository/packages/MathiasDecrock-SeedTotem-4.2.0.zip
              ,https://cdn.thunderstore.io/live/repository/packages/ValheimPlus-ValheimPlus-9.9.8.zip
              ,https://cdn.thunderstore.io/live/repository/packages/OdinPlus-OdinShip-0.0.7.zip
              ,https://cdn.thunderstore.io/live/repository/packages/Detalhes-CustomSpawners-1.0.5.zip
              ,https://cdn.thunderstore.io/live/repository/packages/KGvalheim-Marketplace_And_Server_NPCs_Revamped-7.3.5.zip
              ,https://cdn.thunderstore.io/live/repository/packages/Smoothbrain-CreatureLevelAndLootControl-4.4.7.zip
              ,https://cdn.thunderstore.io/live/repository/packages/Server_devcommands-1.17.0.zip
              ,https://cdn.thunderstore.io/live/repository/packages/Advize-PlantEverything-1.11.2.zip           
                
                
    volumes:
      - ./valheim/saves:/home/steam/.config/unity3d/IronGate/Valheim
      - ./valheim/server:/home/steam/valheim
      - ./valheim/backups:/home/steam/backups

    