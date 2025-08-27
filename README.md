# 👋 Hey, I’m Hasan Zaidi

💻 **Lead iOS Engineer**
I build and scale iOS apps with **Swift, SwiftUI, UIKit, Combine, Core Data, and modern concurrency**. My repos are focused on **clean architecture, developer tooling, and real-world iOS patterns**.

---

## 🛠 Current Stack

```swift
// Languages & Frameworks
Swift • SwiftUI • UIKit • Combine

// Architectures
MVVM • MVVM-C • VIPER • Modularization

// System APIs
Core Data • CloudKit • Core Location • Core Bluetooth • LocalAuthentication • APNs

// Infra & Tooling
CI/CD (GitHub Actions, Fastlane) • Release Automation • Monitoring (Sentry, Datadog)
```

---

## 📂 Highlighted Projects

* ✈️ **Flight Tracker (SwiftUI + AeroDataBox API)**
  Live arrivals/departures, MapKit integration, async/await networking

* 🛒 **Grocery List with iCloud Sync**
  Shared CloudKit data across devices, offline-first, SwiftUI MVVM

* ✅ **ToDo App with Core Data**
  Local persistence, Combine publishers for live updates

* 🏦 **Banking Modules** (enterprise work)
  Modular SwiftUI + UIKit, secure auth flows, accessibility compliance

---

## ⚡️ Swift Snippets

**Combine + Networking**

```swift
apiClient.fetchFlights()
    .receive(on: DispatchQueue.main)
    .sink(receiveCompletion: { print($0) },
          receiveValue: { flights in
              self.flights = flights
          })
    .store(in: &cancellables)
```

**Swift Concurrency**

```swift
func loadFlights() async throws -> [Flight] {
    let (data, _) = try await URLSession.shared.data(from: endpoint)
    return try JSONDecoder().decode([Flight].self, from: data)
}
```

---

## 📊 GitHub Stats

![Hasan's GitHub stats](https://github-readme-stats.vercel.app/api?username=HasanZaidi\&show_icons=true\&theme=tokyonight)

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=HasanZaidi\&layout=compact\&theme=tokyonight)

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=HasanZaidi\&theme=tokyonight)

---

## 🧑‍💻 What I’m Into

* Migrating UIKit → SwiftUI in production apps
* Building **developer productivity tools** (CI/CD, modularization, automation)
* Deep dives on **performance, security, and offline-first design**
* Mentoring iOS engineers on **Swift Concurrency & Combine**

✨ *If you’re into iOS, SwiftUI, or mobile infrastructure — you’ll probably find something useful in my repos.*

---

👉 You’ll just need to replace `HasanZaidi` with your actual **GitHub username** in the badge links above.

Do you also want me to add **badges for tools/skills** (like Swift, SwiftUI, iOS, Fastlane) at the top in a nice row? That gives it more of a **developer CV feel**.
