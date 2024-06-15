# APIJS
+ api.executecommand(); выполняет команду от именни игрока
# CameraJS
+ camera.setCamera(1,2,3,4,5,6,7,8,9,0.01); устонавиливает камеру в 1 2 3 и плавно плывёт к 4 5 6 смотря 7 8 9 со скорость 0.001
+ camera.resetCamera() ресетует камеру
# NpcJS
+ var idnpc = npcJS(0,-60,0,"npc.png","name"); регистрирует NPC с позицией 0 -60 0 с текстурой npc и ником name
+  idnpc.create(); создаёт
+  idnpc.delete(); удаляет
+  idnpc.kill(); убивает
+  idnpc.moveToPosition(1,2,3,4); заставляет идти на 1 2 3 со скоростью 4
+  idnpc.moveToPositionbehindPlayer(1); следовать за игроком с скоростью 1
+  idnpc.playAnim("test"); воспроизводит анимацию
+  idnpc.stopAnim(); останавливает
+  idnpc.setGeo("npc.geo.json"); установить модельку
+  idnpc.setTextures("npc.png"); установить текстуру
+  idnpc.setAnimIdle("test"); заменить анимацию стояния
+  idnpc.setAnimWalk(); заменить анимацию ходьбы
+  idnpc.setName("test"); установить имя
+  idnpc.teleport(1,2,3); телепортировать на 1 2 3
+  idnpc.getX();
+  idnpc.getY();
+  idnpc.getZ();
# NpcJSEvent
+ idnpc.hitNPC(function() { ваш код }); Выполняет при ударе нпс
+ idnpc.interactionsNPC(function() { ваш код }); Выполняет при взаимодействии нпс
