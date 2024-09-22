EN
The code in this Java file represents a simple 2D space game, where the player controls a spaceship that shoots bullets (Ates) at a moving target (likely the red object seen in the screenshot). Here's a breakdown of the game mechanics based on the code:

Classes and Structure:
Ates (Bullet):

The class Ates stores the position (x, y) of each bullet fired by the spaceship. It has getter and setter methods to access or modify its coordinates.
Oyun (Game):

The main game class Oyun extends JPanel and implements KeyListener and ActionListener.
A Timer is used to control the game loop, triggering actions every 5 milliseconds.
The game tracks elapsed time (gecen_sure) and bullets fired (harcanan_ates).
The spaceship (uzayGemisiX) moves horizontally, and bullets are fired when the player presses a key.
The target, which is probably the red circle from the screenshot, moves horizontally across the screen (topX, topdirX).
The player's goal is to hit the moving target with bullets.
Key Mechanics:
Shooting: When the player presses the shoot key (likely spacebar), a new Ates object (bullet) is added to the list atesler.
Collision Detection: The method kontrolEt() checks for collisions between the bullets and the target using rectangles (Rectangle). If a collision occurs, the game ends with the player winning.
Movement:
The spaceship can move horizontally, and the target moves back and forth.
Bullets travel upward until they either hit the target or go off-screen.
Game Objective:
The player wins when they hit the moving target with a bullet. The message displayed in the screenshot says:
"Kazandınız" (You won)
"Harcanan ateş" (Bullets used): 21
"Geçen süre" (Time elapsed): 31.63 seconds
TR
Bu Java dosyasındaki oyun basit bir 2D uzay oyunudur. Oyuncu, bir uzay gemisini kontrol ederek hareket eden bir hedefe ateş eder. Aşağıda oyunun mantığını ve işleyişini açıklıyorum:

Sınıflar ve Yapı:
Ates (Mermi):

Ates sınıfı, uzay gemisinin ateşlediği mermilerin pozisyonlarını (x, y) tutar. Bu sınıf, merminin koordinatlarını almak veya değiştirmek için kullanılan "getter" ve "setter" metodlarına sahiptir.
Oyun (Game):

Ana oyun sınıfı Oyun, JPanel'i genişletir ve KeyListener (klavye dinleyicisi) ve ActionListener (aksiyon dinleyicisi) arabirimlerini uygular.
Bir Timer (Zamanlayıcı), oyun döngüsünü kontrol eder ve her 5 milisaniyede bir oyun içindeki olayları tetikler.
Oyun sırasında geçen süreyi (gecen_sure) ve kullanılan ateş sayısını (harcanan_ates) takip eder.
Uzay gemisi (uzayGemisiX), yatay eksende hareket eder ve oyuncu tuşa bastığında ateş eder.
Hedef, ekranda sağa sola doğru hareket eder (topX, topdirX).
Oyuncunun amacı, hareket eden hedefe mermi ile isabet ettirmektir.
Ana Mekanikler:
Ateş Etme: Oyuncu ateş tuşuna (muhtemelen boşluk tuşu) bastığında, atesler listesine yeni bir Ates nesnesi (mermi) eklenir.
Çarpışma Kontrolü: kontrolEt() yöntemi, mermilerin hedefle çarpışıp çarpışmadığını Rectangle (Dikdörtgen) nesnesi kullanarak kontrol eder. Bir çarpışma olduğunda, oyun biter ve oyuncu kazanır.
Hareket:
Uzay gemisi yatay eksende hareket edebilir ve hedef de ekranda sağa sola hareket eder.
Mermiler yukarı doğru hareket eder ve ya hedefe çarpar ya da ekrandan çıkar.
Oyunun Amacı:
Oyuncu, hareket eden hedefi bir mermi ile vurduğunda kazanır. Ekran görüntüsündeki mesajda şu ifadeler yer alıyor:
"Kazandınız" (Oyunu kazandınız)
"Harcanan ateş" (Kullanılan mermi sayısı): 21
"Geçen süre" (Toplam geçen süre): 31.63 saniye
Bu açıklamalara dayanarak, oyuncu uzay gemisini sağa sola hareket ettirip hedefi vurana kadar ateş etmeye devam eder. Oyunun temel amacı bu.
