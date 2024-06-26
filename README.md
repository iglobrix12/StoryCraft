# APIJS
+ api.executeStory("test story"); выполняет историю
+ api.playerX(); возрощает позицию x игрока
+ api.playerY(); возрощает позицию y игрока
+ api.playerZ(); возрощает позицию z игрока
+ api.playerName(); возрощает имя игрока можно вызывать player.sendMessage("???","привет " + api.playerName());
+ api.worldName(); возрощает имя мира
+ api.setBlock(block.TNT,0,-60,0); ставит блок в мире
+ api.cannot(); делает чтобы игрок не мог ломать блоки
+ api.allow(); делает чтобы игрок мог ломать блоки
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
+ idnpc.performActionBeforeDistance(function() { // ваш код },5 // дистанция); // выполняет если игрок подходит к нпс на 5 блоков
+ idnpc.hitNPC(function() { ваш код }); Выполняет при ударе нпс
+ idnpc.interactionsNPC(function() { ваш код }); Выполняет при взаимодействии нпс
# Events
+ EventBlockClic.setBlock(function() { // ваш код },block.TNT); срабатывает когда игрок кликает по определёному блоку (динамит)
+ EventBlockBreak.setItem(function() { // ваш код },item.TNT); срабытывет когда ломает блок держа предмет в руке (динамит)
+ ItemToss.addItem(functuin() { // ваш код },item.TNT); срабатывает когда игрок выбрасывает предмет (динамит)
+ DealEventPlayer.addEvent(function() { // ваш код }); // срабатывает когда игрок умирает
+ AttackEventPlayer.addEvent(function() { // ваш код )); // срабатывает когда игрок получает урон
+ BlockEvent.BlockBreak(function() { // ваш код }); // срабатывает когда игрок ломает блок
# Overlay
+ overlay.openOverlay(); открывает чёрный экран
+ overlay.closeOverlay(); закрывает чёрный экран
# Player
+ player.sendMessage("text"); отправляет в чат сообщение
+ player.sendMessage("???","text"); отправляет в чат сообщение с ником
+ player.teleport(0,-60,0); телепортирует игрока 
+ player.kill(); убивает игрока
# Dialog
+ DialogManager.addKey1(function() { },"TEXT"); // создаёт кнопку
+ DialogManager.open(); // открывает диалог
+ DialogManager.setVop("TEXT"); // задаёт вопрос
# 1.2.5
