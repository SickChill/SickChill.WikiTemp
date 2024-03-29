## What are Scene exceptions.?

Scene exceptions are alternative names that are used by the "scene" (release groups and uploaders of shows).
Sometimes a show is called differently by the indexer (TheTVDB) than the torrents/nzb's files.
For example, a show is called `Pawn Star$` on the indexer, but the uploaded files are named `Pawn Stars`
When this is the case SickChill can't detect the torrents/nzb's files and they will be skipped. Then a scene exception is the solution.

To add a Scene exception go to the Show and click on the edit button. You will see a field called `scene exception`. Add the desired scene name and save the settings.
On the next search, SickChill will use the newly added scene exception name in its search and should find the show/episodes.

We have tried to automate this process as much as we could by adding scene exception lists. So for known problematic shows, SickChill does automatically add those names.
However, there are still shows that require manually adding the scene exception name.
So when you have a show that requires a manual scene exception please submit a Pull Request to the scene exception list at [SickChill.GitHub.io](https://github.com/SickChill/sickchill.github.io/blob/master/sb_tvdb_scene_exceptions/exceptions.txt). This also helps other users that experience this problem.

![name](images/name.png)

## What is Scene numbering?

Sometimes release groups and uploaders use different episode numbers than an indexer like TheTVDB does. When that happens SickChill can have problems downloading the correct episode.
To get around that problem there is the possibility to add Scene numbers.
This can be done manually or automatically. For manually you need to enable the `Scene` column on the show page. To do that open the show and press the `select column` button and select the `Scene` option. Now you will see a small field in front of every episode. Here you can manually add the scene number.
Automatic adding of scene numbers is done with the help of http://thexem.de
If you take the show `Pawn Stars` for example http://thexem.de/xem/show/1759 you see that different episode numbers are used by the indexers, but thexem.de renumbers/links them to the correct numbers so that SickChill can find the episode.
If there are problematic shows that use a different numbering scheme then please consider adding those on thexem.de so that other users can also profit from the change and don't need to manually add it locally.

![number](images/number.png)
