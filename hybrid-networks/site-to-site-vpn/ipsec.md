## How IP Sec Works
https://www.ciscopress.com/articles/article.asp?p=25474&seqNum=7


How IPSec Works
IPSec involves many component technologies and encryption methods. Yet IPSec's operation can be broken down into five main steps:

1. "Interesting traffic" initiates the IPSec process. Traffic is deemed interesting when the IPSec security policy configured in the IPSec peers starts the IKE process.

2. IKE phase 1. IKE authenticates IPSec peers and negotiates IKE SAs during this phase, setting up a secure channel for negotiating IPSec SAs in phase 2.

3. IKE phase 2. IKE negotiates IPSec SA parameters and sets up matching IPSec SAs in the peers.

4. Data transfer. Data is transferred between IPSec peers based on the IPSec parameters and keys stored in the SA database.

5. IPSec tunnel termination. IPSec SAs terminate through deletion or by timing out.

