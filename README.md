# fast-debian-mirror-selector
Finds the best Debian mirror for a location.

The script finds the best Debian mirror for a location by measuring response time of a list of mirrors stored in arrays. The naming convention for arrays is 'country/territory_name_mirrors' for example Denmark_mirrors, France_mirrors. It iterates through mirrors, pinging each once, and records response time. It then selects the fastest mirror, prints its URL and outputs it.

## User's guide

### Downloading the script

The script can be downloaded by cloning this repository: `git clone https://github.com/Isaac-PM/fast-debian-mirror-selector`, or by using a third-party service like [DownGit](https://minhaskamal.github.io/DownGit/#/home).

### Running the script

Depending in the script was dowloades, it may need to be extracted first. 

After that is done, the script needs to be made executable by running `chmod +x fast-debian-mirror-selector.sh` in the terminal.

Finally, it can be run by executing `./fast-debian-mirror-selector.sh` in the terminal.

### Using the script

The script will print a numbered list of countries/territories, like this one:

```
1. Afghanistan
2. Albania
3. Algeria
4. ...
```
<center><img   src="https://i.imgur.com/yFeyfFz.png"   width=""   height=""   /></center>

For selecting the countries that would like to be teste, the user needs to type the numbers of the countries, separated by commas, and press enter. For example, if the user wants to test the mirrors in the Albania and Algeria, they would type `1, 2` and press enter.

<center><img   src="https://i.imgur.com/InbKgRm.png"   width=""   height=""   /></center>

Then the script will `ping` each mirror in the selected countries, and print the results. After that, it will print the URL of the fastests mirrors.

<center><img   src="https://i.imgur.com/ClgL9IB.png"   width=""   height=""   /></center>
