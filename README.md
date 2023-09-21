# moebel_de_coding_challenge

# Build
- run `flutter pub get`

# Steps Taken
1. import riverpod packages
2. wrap app with ProviderScope
3. make a FutureProvider that returns the Products
4. change MyHomePage to stateless Widget
5. add Riverpods Widget Consumer to the Scaffold so there is access to WidgetRef and thus access to the glboal productsProvider
6. use ref.watch(productsProvider) to fetch Data
7. ref.watch return an AsyncValue that idicates if it is loading, has an error or the data is there and updates automatically as soon as changes are noticed
   thus triggering the rebuild of that specific UI that implements the Consumer
8. Make an Widget for displaying the products and pass Products as Parameter
9. Show CircularProgressIndicator while loading data
10. Show Error when an error occurs



