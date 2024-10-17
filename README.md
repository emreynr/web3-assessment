# web3-assessment

> [!NOTE]  
> İlgili bütün kodlar ve kontrol edilebileceği bir link aşağıda belirtilmiştir. <br /> <br />
Kullanılan Dil: Motoko <br /> <br />

```Motoko
// Hesap Makinesi
// Degiskenler ->> let: sabit, var: degistirilebilir
// Operatorler
// Async Metodu
// If Kosulu

// Canister ->> Akilli Kontratlar

actor hesap_makinesi {
  var hucre: Int = 0;

  // toplama
  public func toplama(s: Int) : async Int {
    hucre += s;
    hucre
    // bu kod ile output gorulebilir
    //Debug.print(debug_show (hucre));
  };

  // cikarma
  public func cikarma(s: Int) : async Int {
    hucre -=s;
    hucre
  };

  //carpma
  public func carpma(s: Int) : async Int {
    hucre *= s;
    hucre
  };

  // bolme
  public func bolme(s: Int) : async ?Int {
    if (s == 0) {
      null
    } else {
      hucre /=s;
      ?hucre
    }
  };

  // temizle
    public func temizle() : async () {
      hucre := 0;
    };
};
``` 
<br />

*Kodları kontrol etmek için [tıklayın](https://m7sm4-2iaaa-aaaab-qabra-cai.raw.ic0.app/?tag=1783318918)* 
