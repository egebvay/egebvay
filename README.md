
 cProfile  içe  aktarma çalıştırmasından
playound'dan  playsound'u  içe  aktar
gtts'den  gTTS'yi  içe  aktar
 konuşma_recognition'ı  sr olarak  içe aktar
 işletim sistemini içe aktar
ithalat  zamanı
 datetime  ithalat  tarihinden itibaren , datetime
 rastgele içe aktar
 rastgele  içe  aktarma seçiminden
pydub'dan  AudioSegment'i  içe  aktarın
web tarayıcısını içe  aktar

r  =  sr . tanıyıcı ()


# def hızlanma():
# in_path = 'answer.mp3'
# ex_path = 'speed.mp3'
# ses = AudioSegment.from_file(in_path)
# slower_sound = speed_swifter(ses, 1.3)
# slower_sound.export(ex_path, format="mp3")

# def speed_swifter(ses, hız=1.0):
# sound_with_altered_frame_rate = sound._spawn(sound.raw_data, overrides={"frame_rate": int(sound.frame_rate * hız)})
# sound_with_altered_frame_rate döndür


def  kaydı ( ask = False ):
     sr ile . Kaynak olarak mikrofon () : 
        sorarsanız  : _
            yazdır ( sor )
        ses  =  r . dinle ( kaynak )
        ses  =  ""
        dene :
            ses  =  r . tanıma_google ( ses , dil = "tr-TR" )
         sr hariç . BilinmeyenDeğerHatası :
            print ( "Asistan: Anlayamadım" )
         sr hariç . İstek Hatası :
            print ( "Asistan: Sistem çalışmıyor" )
        dönüş  sesi


def  yanıtı ( ses ):
     " merhaba "  sesinde  ise :
        konuş ( "sana da merhaba genç" )
     sesinde " selam"  ise : 
        konuş ( "sana 2 kere selam olsun" )
     sesle " teşekkür ederim"  veya sesle " teşekkürler" ise  :    
        konuş ( "rica ederim" )
     sesinde "görüşürüz  " ise : 
        konuş ( "görüşürüz canım" )
        çıkış ()

     sesinde " hangi gündeyiz"  ise : 
        bugün  =  zaman . strftime ( "%A" )
        bugün . büyük harf yap ()
        if  bugün  ==  "Pazartesi" :
            bugün  =  "Pazartesi"

        elif  bugün  ==  "Salı" :
            bugün  =  "Salı"

        elif  bugün  ==  "Çarşamba" :
            bugün  =  "Çarşamba"

        elif  bugün  ==  "Perşembe" :
            bugün  =  "Perşembe"

        elif  bugün  ==  "Cuma" :
            bugün  =  "Cuma"

        elif  bugün  ==  "Cumartesi" :
            bugün  =  "Cumartesi"

        elif  bugün  ==  "Pazar" :
            bugün  =  "Pazar"

        konuşmak ( bugün )

     sesinde "saat kaç  " ise : 
        seçim  = [ "Saat şu an:" , "Hemen çıkıyor: " ]
        saat  =  tarihsaat . şimdi (). strftime ( "%H:%M" )
        seçim  =  rastgele . seçim ( seçim )
        konuş ( seçim  +  saat )

     "google'da ara  "  sesli ise :
        konuş ( "Ne aramamı istersin?" )
        arama  =  kayıt ()
        url  =  "https://www.google.com/search?q={}" . biçim ( arama )
        web tarayıcısı . () alın . aç ( url )
        konuş ( "{} içi Google'da bulabildiklerimi listeliyorum." . format ( arama ))

     seste "uygulama aç "  ise : 
        konuş ( "Hangi hazırlamamı?" )
        runApp  =  kayıt ()
        runApp  =  runApp . alt ()
        runApp  içinde "valorant"  ise : 
            os . startfile ( "D:\Riot Games\Riot Client\RiotClientServices.exe" )
            konuş ( "İstediğin paketi çalıştırıyorum." )
        elif  runApp'de "hayat garip  " : 
            os . startfile ( "steam://rungameid/319630" )
            konuş ( "İstediğin paketi çalıştırıyorum." )
        başka :
            konuş ( "İstediğin uygulama çalıştırma listemde yok." )

def  konuş ( dize ):
    tts  =  gTTS ( metin = dize , lang = "tr" , yavaş = Yanlış )
    dosya  =  "cevap.mp3"
    tts . kaydet ( dosya )
    # hızlanma()
    çalma sesi ( dosya )
    os . kaldırmak ( dosya )
    # os.remove("speed.mp3")

def  testi ( uyandırma ):
    eğer  "charlie  " uyanırsa : 
        çalma sesi ( " DING.mp3 " )
        uyan  =  kaydet ()
        eğer  uyan  !=  '' :
            ses  =  uyan . alt ()
            print ( uyandır . büyük harf kullan ())
            cevap ( ses )


# konuş("Selam madenci")
çalma sesi ( " DING.mp3 " )

 Doğru iken :
    uyan  =  kaydet ()
    eğer  uyan  !=  '' :
        uyanmak  =  uyanmak . alt ()
        print ( uyandır . büyük harf kullan ())
        sınamak ( uyanmak )
