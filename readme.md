![VVVVID-Downloader](https://socialify.git.ci/CoffeeStraw/VVVVID-Downloader/image?description=1&descriptionEditable=Un%20piccolo%20script%20in%20Python3%20per%20scaricare%20contenuti%20multimediali%20(non%20a%20pagamento)%20offerti%20da%20VVVVID&font=KoHo&forks=1&issues=1&language=1&owner=1&pattern=Charlie%20Brown&stargazers=1&theme=Dark)

---

## NOTE
This project is no longer maintained, as VVVVID has been closed. Thank you all for your support.

## 📚 Description
**VVVVID Downloader** is a convenient solution for downloading content from the well-known **VVVVID** site, all you need is the **link** to the series/film or a single episode, it will do the rest.
In particular, there are two cases for links:
- Link to **single episode**: the script will download from that episode onwards, only the episodes of that season.
- Link to **film/anime page** with episode list: the script will download all episodes of all available seasons or the single film.

During development, we chose to adopt these conventions because they turned out to be the most convenient for everyday use. The project is however open to alternative solutions and it is possible to discuss them by opening an issue.

## ⚙️ Installation
### Release (Windows)
Download [the latest release](https://github.com/CoffeeStraw/VVVVID-Downloader/releases). You will end up with a *.zip*, which you will have to unpack. To start the program, simply launch "VVVVID Downloader.bat".

### Docker
To install and use the software via **Docker**, simply launch the file ```vvvvvid-downloader.sh```. It will take care of launching the container and will mount the *Downloads* folder as an external volume.

## 🎮 Usage
To use VVVVID Downloader, all you have to do is put the link to what you want to download from VVVVID inside the **downloads_list.txt** file, which already contains examples.
## ℹ️ Note:
- If you have multiple links, each one should be placed on a separate line.
- Lines starting with **#** will be ignored, it can be useful if you want to temporarily ignore something for example.
- For copyright reasons VVVVID is not available abroad, so you need to have an Italian IP address.

## 👨‍💻 Developers - Release Windows
To create the Windows executable **pyinstaller** is used. The steps are as follows:
- Create a virtual environment with ```venv``` and activate it;
- Install the requirements and install ```pyinstaller``` with **pip**;
- Produce the executable with the command:
```sh
pyinstaller -F main.py
```
- Add to the executable the files ```downloads_list.txt``` and ```VVVVID Downloader.bat```, which you can find in old releases;
- Move the executable to a new folder called ```bin/```;
- Include in the ```bin/``` folder also the executable of ```ffmpeg```.

## 🧭 License
This software is distributed under the MIT license. Read the `LICENSE` file for more information.
