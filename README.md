BottomSheet
=======

Bottom Sheets

One way to present a set of actions to a user is with bottom sheets, a sheet of paper that slides up from the bottom edge of the screen. Bottom sheets offer flexibility in the display of clear and simple actions that do not need explanation.

[url|https://www.google.com/design/spec/components/bottom-sheets.html]

This library works on android 2.1+ (not verify yet)

Under heavy development, methods would change at any moment without notice, please do not use it in productive enviorment now.

![Sample](https://github.com/soarcn/BottomSheet/blob/master/art/image.png?raw=true)

How to use this library
=======

- Download this library, import to your IDE (eclipse...) as a library project.
- Using Gradle (will be available soon)

    ```groovy
    compile 'com.cocosw:bottomsheet:0.+@aar' 
    ```


API
=======

- Define actions in menu xml

```java
new BottomSheet.Builder(this).title("title").xml(R.menu.list).listener(new DialogInterface.OnClickListener() {
                    @Override
                    public void onClick(DialogInterface dialog, int which) {
                        switch (which) {
                            case R.id.help:
                                q.toast("Help me!");
                                break;
                        }
                    }
                }).show();

```
- You can also add action items in builder.

Contribute
=======

- Feel free to fork it

TODO
=======
- Screen rotation
- Dark theme
- Grid view
- Uploading to centre repository
- Style/animation tweaking
- L style support
- Style customization


License
=======

    Copyright 2011, 2014 Liao Kai

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
