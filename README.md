![[Mobile System Design.png]]

## **Mobile Domain**

### **UI Frameworks**
- **Declarative**
	- **iOS: SwiftUI**
	- **Android: Jetpack Compose**
- **Imperative**
	- **iOS: UIKit**
	- **Android: View System (XML / Code)**

### **Lifecycle Management**
- **iOS: UIViewController, AppDelegate, SceneDelegate**
- **iOS: SwiftUI View**
- **Android: Activity, Fragment, Application**
- **Android: Jetpack Compose**

### **Threading & Concurrency**
- **iOS: GCD, Operation Queue, async/await, Tasks, Actors**
- **Android: Looper, Handler, ThreadPoolExecutor, Coroutines**

### **Navigation**
- **iOS: UINavigationController, SwiftUI NavigationStack**
- **Android: Navigation Component**
- **Coordinator patterns**
- Deep Links

### **Data Binding**
- **iOS: Completion handlers, Combine, KVO, ObservableObject**
- **Android: LiveData, Kotlin Coroutines (Flow/StateFlow)**

### Runtime
- Android VM & Runtime
- iOS Runtime

## **API Design & Networking**

### **Communication Protocols**
- **REST**
- **Websockets**
- GraphQL
- gRPC

### **Real-time Updates**
- **HTTP Polling**
- **HTTP Long-Polling**
- **Server-Sent Events (SSE)**
- **WebSockets**
- **Push Notifications**

### **Pagination**
- **Limit-Offset Pagination**
- **Page-Based Pagination**
- **Keyset Pagination**
- **Cursor-Based Pagination**

### **API Integration**
- **HTTP Clients**
	- **iOS: URLSession, Alamofire**
	- **Android: OkHTTP, Retrofit**
- **Serialization & Parsing**
	- **iOS: Codable /   
	  Decodable**
	- **iOS: JSONDecoder / JSONEncoder customisation**
	- **Android: Moshi / Gson**
	- **DTO & Domain model mappers**
- **Background Calls**
	- **iOS: URLSession background session**
	- **Android: WorkManager, JobScheduler**
- **Delta Updates**
	- **Using Timestamps**
	- **Using SequenceID**
	- **Using ETAG**
- Offline & Sync
	- Conflict resolution
	- Queueing
	- Background retry
- Batched Requests
- Resumable Uploads / Downloads
- Prefetching

### **Caching Strategies**
- **HTTP Cache-Control  
  Headers**
- **ETag / Last-Modified**
- **Memory Cache**
	- **iOS: NSCache**
	- **Android: LRUCache**
- **Disk Cache**
- Custom Cache Invalidation Strategies

### Authentication
- Basic Login/Password over HTTPS
- Third-Party Logins
	- Sign in with Apple / Google
	- OAuth 2.0
	- OpenID
- Multi-Factor Authentication
- Access Token & Refresh Token Flow
- Token storage best practices

### Retry Policies
- Exponential Backoff
- Linear Backoff
- Circuit Breakers
- Retrying after OAuth token refresh

### API Evolution & Backward compatibility
- URI Versioning
- Adding / Removing fields

### CDN

## **Software Architecture & Design Patterns**

### **App-Wide Architectural patterns**
- **MVC**
- **MVP**
- **MVVM**
- **MVI**
- **Clean Architecture**
- VIPER
- Redux

### **Design Patterns (GO4)**
- **Creational**
	- **Singleton**
	- **Factory Method**
	- **Builder**
	- Abstract Factory
	- Prototype
- **Structural**
	- **Facade**
	- **Proxy**
	- **Adapter**
	- **Decorator**
	- Composite
	- Bridge
	- Flyweight
- **Behavioral**
	- **Observer**
	- **Chain of responsibility**
	- Strategy
	- Mediator
	- Command
	- Memento
	- Interpreter
	- Visitor

### **Other**
- **Dependency Injection**
	- **iOS: Manual DI in Swift**
	- **Android: Manual DI in Kotlin**
	- iOS: Swinject
	- Android: Hilt, Dagger
- **Delegate**
- **Reactive Programming**
- Service Locator
- Feature flags & Remote Config

## **Data Storage**

### **Key-Value Storage**
- **iOS: UserDefaults**
- **Android: SharedPreferences, Preferences DataStore**

### **Database**
- **SQLite**
- **Realm**
- **iOS: CoreData**
- **Android: Room**
- **ObjectBox**

### **Secure Storage**
- **iOS: Keychain**
- **Android: EncryptedSharedPreferences, Jetpack Security**

### **File Storage**

### Binary Storage
- Android: Proto DataStore

## **Performance & Optimization**

### **Memory Management**
- **Common Leak Sources**
- Leak Detection
- Profiling & Metrics

### **CPU & Battery**
- **Background Task Scheduling**
- **Power-Saving modes**
	- **iOS: App Nap**
	- **Android: Doze Mode**

### Rendering & Animation

### App Startup Time

### Optimize Geo-Location Usage

### App Size

## **Observability & Testing**

### **Unit Testing**
- **iOS: XCTest**
- **Android: JUnit**

### **Mocking Frameworks**
- **iOS: Mockingbird**
- **Android: Mockito**

### **Integration Testing**

### **UI Testing**
- **iOS: XCUITest, EarlGrey 2.0, Snapshot Test**
- **Android: Espresso, UI Automator**

### **CI / CD**

### E2E Testing
- Detox, Appium

### Beta Distribution & Rollouts

### Logging & Monitoring

### Metrics & Dashboards

### Crash Reporting

## **Privacy & Security**

### **Data Encryption**

### **Secure Storage**

### Minimize Data Collection

### Minimize Permission Usage

### Data Retention & Deletion

### Code security, integrity, obfuscation

### Privacy Compliance

## **Advanced Topics**

### On-Device Machine Learning

### Augmented & Virtual Reality

### Wearables

### Foldables & Multi-Window UIs

### Server-Driven UI

### Cross-Platform Mobile Development

### Internationalization

## **Interview Strategy (Non Tech)**

### **Lead the conversation**

### **Clarify requirements**
- **Ask questions to reduce ambiguity**
- **Determine scope: client, API, backend**
- **Define functional requirements**
- **Define non-functional requirements**
	- **Offline mode**
	- **Minimise traffic bandwidth**
	- Minimize battery consumption
	- Optimize scroll: FPS = 60
	- Data consistency: strong vs eventual
	- Address scale of the engineering team
- **Define out of scope**
- **Address scale**
	- **DAU: Daily Active Users**
- Address authentication
- Address target OS versions

### **Problem Navigation**
- **Structural approach: Requirements, Data Model & API, High Level Design, Deep Dives**
- **Prioritize: solve most important problems**
- **BFS then DFS**
- **Foresee common problems**
- Learn Basics of C4 model

### **Communicate Effectively**
- **Organise information in a logical way**
- **Bring relevant context**
- Make complex topics easily digestible

### **Articulate trade-offs**
- **Communicate benefits of your design choice**
- **Bring up multiple solutions and assess their pros and cons**
- Articulate conflicting approaches with pros/cons

### **Engage with Interviewer**
- **Listen carefully**
- **React to feedback and questions**
- **Deep dive if requested**
- **Be ready to accept your mistakes and fix them**
