# SwiftUI Admob Guide
![Swift](https://img.shields.io/badge/Swift-5.9-orange.svg)
![Platform](https://img.shields.io/badge/Platform-iOS17%20-red.svg)
![Platform](https://img.shields.io/badge/SwiftUI-4-green.svg)
![License](https://img.shields.io/badge/License-MIT-blue.svg)

[<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8c/Google_AdMob_logo.svg/1280px-Google_AdMob_logo.svg.png">](https://durmaz.notion.site/SwiftUI-Admob-Rehberi-0b531e7be21f4d83a37214c62d2cc637 "SwiftUI Admob Guide")

1. **Admob SDK Installation**
    1. Xcode with SPM → Add Package Dependencies
        
        ```swift
        https://github.com/googleads/swift-package-manager-google-mobile-ads.git
        ```
        
    2. Adding Application Identifier and SKAdNetworkIdentifier to Info.plist file
        
        ```swift
        <?xml version="1.0" encoding="UTF-8"?>
        <!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
        <plist version="1.0">
        <dict>
            <key>GADApplicationIdentifier</key>
            <string>admob-app-identifier</string> //start with ca-app-pub
            <key>SKAdNetworkItems</key>
            <array>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>cstr6suwn9.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>4fzdc2evr5.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>4pfyvq9l8r.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>2fnua5tdw4.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>ydx93a7ass.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>5a6flpkh64.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>p78axxw29g.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>v72qych5uu.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>ludvb6z3bs.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>cp8zw746q7.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>3sh42y64q3.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>c6k4g5qg8m.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>s39g8k73mm.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>3qy4746246.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>f38h382jlk.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>hs6bdukanm.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>v4nxqhlyqp.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>wzmmz9fp6w.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>yclnxrl5pm.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>t38b2kh725.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>7ug5zh24hu.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>gta9lk7p23.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>vutu7akeur.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>y5ghdn5j9k.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>n6fk4nfna4.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>v9wttpbfk9.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>n38lu8286q.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>47vhws6wlr.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>kbd757ywx3.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>9t245vhmpl.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>eh6m2bh4zr.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>a2p9lx4jpn.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>22mmun2rn5.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>4468km3ulz.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>2u9pt9hc89.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>8s468mfl3y.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>klf5c3l5u5.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>ppxm28t8ap.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>ecpz2srf59.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>uw77j35x4d.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>pwa73g5rt2.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>mlmmfzh3r3.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>578prtvx9j.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>4dzt52r2t5.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>e5fvkxwrpn.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>8c4e2ghe7u.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>zq492l623r.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>3rd42ekr43.skadnetwork</string>
              </dict>
              <dict>
                <key>SKAdNetworkIdentifier</key>
                <string>3qcr597p9d.skadnetwork</string>
              </dict>
            </array>
        </dict>
        </plist>
        ```
        
    3. Calling the Admob SDK in the startup file of the SwiftUI application
        
        ```swift
        import SwiftUI
        import GoogleMobileAds
        
        @main
        struct KPSS_Puan_HesaplamaApp: App {
            
            init() {
                // Admob SDK
                GADMobileAds.sharedInstance().requestConfiguration.testDeviceIdentifiers = [ "c458ae01182d2fad3701091c1e7991e0" ]
                GADMobileAds.sharedInstance().start(completionHandler: nil)
                // If you are going to use a test device, you must call it before the start method.
            }
            
            var body: some Scene {
                WindowGroup {
                    ContentView()
                }
            }
        }
        ```
        
2. **Banner ADS:**
    
    ```swift
    import Foundation
    import UIKit
    
    protocol BannerViewControllerWidthDelegate: AnyObject {
      func bannerViewController(_ bannerViewController: BannerViewController, didUpdate width: CGFloat)
    }
    
    class BannerViewController: UIViewController {
      weak var delegate: BannerViewControllerWidthDelegate?
    
      override func viewDidAppear(_ animated: Bool) {
        super.viewDidAppear(animated)
    
        // Tell the delegate the initial ad width.
        delegate?.bannerViewController(
          self, didUpdate: view.frame.inset(by: view.safeAreaInsets).size.width)
      }
    
      override func viewWillTransition(
        to size: CGSize, with coordinator: UIViewControllerTransitionCoordinator
      ) {
        coordinator.animate { _ in
          // do nothing
        } completion: { _ in
          // Notify the delegate of ad width changes.
          self.delegate?.bannerViewController(
            self, didUpdate: self.view.frame.inset(by: self.view.safeAreaInsets).size.width)
        }
      }
    }
    ```
    
    ```swift
    import SwiftUI
    import GoogleMobileAds
    
    struct BannerView: UIViewControllerRepresentable {
        @State private var viewWidth: CGFloat = .zero
        private let bannerView = GADBannerView()
        private let adUnitID = "ca-app-pub-xxxxxx" // Reklam Birimi Identifier
        
        func makeUIViewController(context: Context) -> some UIViewController {
            let bannerViewController = BannerViewController()
            bannerView.adUnitID = adUnitID
            bannerView.rootViewController = bannerViewController
            bannerView.delegate = context.coordinator
            bannerView.translatesAutoresizingMaskIntoConstraints = false
            bannerViewController.view.addSubview(bannerView)
            // Constrain GADBannerView to the bottom of the view.
            NSLayoutConstraint.activate([
                bannerView.bottomAnchor.constraint(
                    equalTo: bannerViewController.view.safeAreaLayoutGuide.bottomAnchor),
                bannerView.centerXAnchor.constraint(equalTo: bannerViewController.view.centerXAnchor),
            ])
            bannerViewController.delegate = context.coordinator
            
            return bannerViewController
        }
        
        func updateUIViewController(_ uiViewController: UIViewControllerType, context: Context) {
            guard viewWidth != .zero else { return }
            
		        let request = GADRequest()
		        // iPad'lerde adaptif reklam boyutları için
              request.scene = UIApplication.shared.connectedScenes.first as? UIWindowScene
              bannerView.load(request)
        }
        
        func makeCoordinator() -> Coordinator {
            Coordinator(self)
        }
        
        internal class Coordinator: NSObject, BannerViewControllerWidthDelegate, GADBannerViewDelegate
        {
            let parent: BannerView
            
            init(_ parent: BannerView) {
                self.parent = parent
            }
            
            // MARK: - BannerViewControllerWidthDelegate methods
            
            func bannerViewController(
                _ bannerViewController: BannerViewController, didUpdate width: CGFloat
            ) {
                parent.viewWidth = width
            }
            
            // MARK: - GADBannerViewDelegate methods
    
            func bannerViewDidReceiveAd(_ bannerView: GADBannerView) {
              print("\(#function) called")
            }
    
            func bannerView(_ bannerView: GADBannerView, didFailToReceiveAdWithError error: Error) {
              print("\(#function) called")
            }
    
            func bannerViewDidRecordImpression(_ bannerView: GADBannerView) {
              print("\(#function) called")
            }
    
            func bannerViewWillPresentScreen(_ bannerView: GADBannerView) {
              print("\(#function) called")
            }
    
            func bannerViewWillDismissScreen(_ bannerView: GADBannerView) {
              print("\(#function) called")
            }
    
            func bannerViewDidDismissScreen(_ bannerView: GADBannerView) {
              print("\(#function) called")
            }
        }
    }
    ```
    
    Contains methods within a class in the AdMob iOS SDK that implements the **`GADBannerViewDelegate`** protocol. These methods are used to receive notifications about the status and interaction of the Google AdMob advertising banner:
    
    1. **`bannerViewDidReceiveAd(_ bannerView: GADBannerView)`**: Banner reklamın başarıyla alındığı ve görüntülendiği zaman bu metot çağrılır.
    2. **`bannerView(_ bannerView: GADBannerView, didFailToReceiveAdWithError error: Error)`**: Banner reklamın yüklenme işlemi başarısız olduğunda bu metot çağrılır. Bir hata nesnesi, hata hakkında daha fazla bilgi sağlar.
    3. **`bannerViewDidRecordImpression(_ bannerView: GADBannerView)`**: Banner reklamın bir izlenim kaydedildiğinde bu metot çağrılır. Banner reklamın görüntülendiği her bir defa bu metot tetiklenir.
    4. **`bannerViewWillPresentScreen(_ bannerView: GADBannerView)`**: Banner reklamın tam ekran bir sayfa veya ekranın bir bölümüyle örtüştüğü bir ekranın sunulması öncesinde bu metot çağrılır. Örneğin, bir kullanıcı reklama tıkladığında ve uygulama bir tarayıcı ekranı veya başka bir uygulama ekranı açtığında bu metot tetiklenir.
    5. **`bannerViewWillDismissScreen(_ bannerView: GADBannerView)`**: Banner reklamın tam ekran bir sayfa veya ekranın örtüştüğü ekranın kapatılması öncesinde bu metot çağrılır.
    6. **`bannerViewDidDismissScreen(_ bannerView: GADBannerView)`**: Banner reklamın tam ekran bir sayfa veya ekranın örtüştüğü ekranın kapatılması sonrasında bu metot çağrılır. Bu metot, reklam ekranının kapatılması işleminin tamamlandığını belirtir.
    
4. **Interstitial ADS:**
    
    ```swift
    import Foundation
    import GoogleMobileAds
    
    class AdCoordinator: NSObject,GADFullScreenContentDelegate {
        private var ad: GADInterstitialAd?
        
        override init() {
            super.init()
            loadAd()
        }
        
        func loadAd() {
            let request = GADRequest()
            request.scene = UIApplication.shared.connectedScenes.first as? UIWindowScene
        
            GADInterstitialAd.load(
                withAdUnitID: "ca-app-pub-xxxx", request: request
            ) { ad, error in
                if let error = error {
                    return print("Failed to load ad with error: \(error.localizedDescription)")
                }
                
                self.ad = ad
                self.ad?.fullScreenContentDelegate = self
                
            }
        }
        
        func presentAd() {
            guard let fullScreenAd = ad else {
                return print("Ad wasn't ready")
            }
            
            // View controller is an optional parameter. Pass in nil.
            fullScreenAd.present(fromRootViewController: nil)
        }
        
        // MARK: - GADFullScreenContentDelegate methods
    
        func adDidRecordImpression(_ ad: GADFullScreenPresentingAd) {
          print("\(#function) called")
        }
    
        func adDidRecordClick(_ ad: GADFullScreenPresentingAd) {
          print("\(#function) called")
        }
    
        func ad(_ ad: GADFullScreenPresentingAd, didFailToPresentFullScreenContentWithError error: Error) {
          print("\(#function) called")
        }
    
        func adWillPresentFullScreenContent(_ ad: GADFullScreenPresentingAd) {
          print("\(#function) called")
        }
    
        func adWillDismissFullScreenContent(_ ad: GADFullScreenPresentingAd) {
          print("\(#function) called")
        }
    
        func adDidDismissFullScreenContent(_ ad: GADFullScreenPresentingAd) {
          print("\(#function) called")
            loadAd()
        }
    
    ```
    
   The **`GADFullScreenContentDelegate`** methods in the AdMob iOS SDK are used to track events related to the delivery of full-screen content by the ad publisher and user interaction. Its functions are as follows:
    
    1. **`adDidRecordImpression(_ ad: GADFullScreenPresentingAd)`**: Reklam gösterim olayının kaydedildiği zaman bu metot çağrılır. Bir reklamın izlenme sayısı gibi metriklerin takibi için kullanılabilir.
    2. **`adDidRecordClick(_ ad: GADFullScreenPresentingAd)`**: Kullanıcının reklama tıkladığı zaman bu metot çağrılır. Kullanıcıların reklamla etkileşimlerinin takibi için kullanılabilir.
    3. **`ad(_ ad: GADFullScreenPresentingAd, didFailToPresentFullScreenContentWithError error: Error)`**: Tam ekran içeriğin sunulamadığı bir hata oluştuğunda bu metot çağrılır. Örneğin, reklam yüklenirken bir ağ hatası oluşabilir.
    4. **`adWillPresentFullScreenContent(_ ad: GADFullScreenPresentingAd)`**: Tam ekran içeriğin gösterilmeye başlanmadan önce bu metot çağrılır. Uygulamanın gerektiği gibi durumunu ayarlamak için kullanılabilir.
    5. **`adWillDismissFullScreenContent(_ ad: GADFullScreenPresentingAd)`**: Tam ekran içeriğin kullanıcı tarafından kapatılmadan önce bu metot çağrılır. Kullanıcı reklamı kapatmaya karar verirse, bu olay tetiklenir.
    6. **`adDidDismissFullScreenContent(_ ad: GADFullScreenPresentingAd)`**: Tam ekran içeriğin kullanıcı tarafından kapatıldıktan sonra bu metot çağrılır. Reklamı kapatma işlemi tamamlandığında kullanılabilir.
    
    These methods allow for better control of full-screen ads by the publisher and tracking of user interactions. In this way, the performance of ads and user experience can be optimized.
    
6. **App Tracking Transparency (tracking permission for Personalized Ads)**
    
   AppTrackingTransparency is an API introduced in iOS 14 and later that requires users to explicitly accept the tracking purpose of apps. This API imposes a consent requirement for apps that track users' devices for advertising and analytics purposes.
   Apps must ask the user for permission using the AppTrackingTransparency API before serving user tracking requests. The user is given an option to accept or decline the app from sharing their personal data with other companies for advertising or data analysis purposes.
   This API ensures that users are informed about tracking and their consent is obtained, providing better control over privacy. This allows users to feel more privacy and security.
   
    1. The following Key and Value are defined in the Info.plist file.
        > Privacy - Tracking Usage Description : Would you allow us to make ads more personalized for you?
        
    2. Permission is requested from the user with the following onReceive modifier in any view or main file of the application.
        
        ```swift
        import SwiftUI
        import AppTrackingTransparency
        
        struct ContentView: View {
            var body: some View {
                VStack{
                    Text("Hello ADMOB!")
                }
                .onReceive(NotificationCenter.default.publisher(for: UIApplication.didBecomeActiveNotification)) { _ in
                    ATTrackingManager.requestTrackingAuthorization(completionHandler: { status in })
                }        
            }
        }
        
        ```
        
    

### **Examples:**

1. **Banner**
    
    ```swift
    import SwiftUI
    import GoogleMobileAds
    
    struct ContentView: View {
        var width: CGFloat = UIScreen.main.bounds.width
    
  	var size: CGSize {
  		return GADCurrentOrientationAnchoredAdaptiveBannerAdSizeWithWidth(width).size
  	} // adaptif reklam boyutları için (iPad uyumluluğu için)

        var body: some View {
            VStack{
                Text("Hello ADMOB!")
                    BannerView()
                        .frame(height: size.height)
            }      
        }
    }
    ```
    
2. **Interstitial**
    
    ```swift
    import SwiftUI
    import GoogleMobileAds
    
    struct ContentView: View {
    	private let adCoordinator = AdCoordinator()
    
        var body: some View {
            VStack{
                Text("Hello ADMOB!")
                    Button("Show Interstitial"){
                        adCoordinator.presentAd()
                }
            }      
        }
    }
    ```
