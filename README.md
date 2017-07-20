# SessionManager-Android
Small Shared Preference Library for Android

# Download

You can download a source code from Github's [releases page](https://github.com/Chingiz/SessionManager-Android/releases/tag/v0.2-beta).

Or use Gradle

Add it in your root build.gradle at the end of repositories:

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
	
Step 2. Add the dependency

	dependencies {
	        compile 'com.github.Chingiz:SessionManager-Android:v0.2-beta'
	}
	
# How do I use SessionManager?
```
@Override
protected void onCreate(Bundle savedInstanceState) {
	...
	SessionManagerDebug sessionManagerDebug = new SessionManagerDebug(getApplicationContext());
        
	sessionManagerDebug.putString("test", "I'm SessionManager");

	Log.d("Main ", "onCreate: "+sessionManagerDebug.getString("test", "1"));
	}
```
# License

MIT licensed, (c) [@hchingiz](http://twitter.com/hchingiz) 

