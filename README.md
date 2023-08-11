# Sol
Sol is a hostile utility for post-exploitation capable of USB/external device cloning and exfiltration. It targets Linux hosts and requires access to a system with RWX caoabilities.

Technique Used: [***MITRE ATT&CK T-1091***](https://attack.mitre.org/techniques/T1091/) -  Replication Through Removable Media. Using the knowledge gained from this technique, we leverage it in a unique way!
## Usage
Sol takes advantage of the techniques learned in [Pilgrim](https://github.com/diante0x7/Pilgrim) to execute wholly in memory. It requires the ability to not only obtain but retain persistence, allowing it to focus on it's goal of monitoring the creation of new drives or network shares, cloning the data and exfiltrating it from the target machine for analysis and parsing.
## Outro
This tool builds upon leveraging Living-Off-The-Land binaries (LOLBins) to perform tasks outside of the scope of the physical hard drive for anti-analysis measures. Sensitive information and various programs are typically transferred or copied onto and from removable media, giving the attacker the ability to stealthily acquire information that they might not have noticed without having to interact or monitor the host manually. Turning a host against itself to perform adversarial tasks such as this opens the door for an attacker to find innovative ways to perform malicious or malign actions without raising suspicion which raises many issues for a security professional!
