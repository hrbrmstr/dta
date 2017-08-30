Data feed & (eventual) blog content for "Delete This App" (<https://deletethisapp.com/>)

-------------

Unlike other places that just provide information, this is a pretty in-your-face type of endeavour. Apps have been around for long enough that developers and publishers should know better. So, rather than just notify of an issue, this is a "delete it now" recommender system. Lonstanding publishers get zero chances, so the `"permanent_remove" : true` flag will be set for them. Nascent ones will be given some slack, but not much.

The database will be platform-agnostic. Offending apps on Windows, macOS, iOS, Linux and even in-browser (like Chrome apps) are fair game. There's too much at stake when it comes to apps on your devices. They know tons about you and more of them than you'd like to know do terrible things with your data. This is one way to fight back.

I'm still working out the schema and it'll likely change, but the idea is to have one JSON file per "public service announcement" (PSA) for app removals on Twitter and auto-gen a Hugo blog from it.

Feel free to contribute app del suggestions via JSON files and schema posits via PRs. If doing the former, use something like `uuid::UUIDgenerate()` (that in R code) to generate a UUID for the JSON entry file name until I get a mini-pkg & Shiny app written.