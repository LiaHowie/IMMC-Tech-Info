---
draft: true
note: A draft page will not be shown in the production site
title: New SSDs
---
Following on from the [[25-11-29|ZFS Storage Pool Troubles?]] post, I've finally managed to replace the DRAMless SSDs with 'DRAM-ful' NVMe SSDs! Whoop! But getting there was, uh, needlessly difficult... 

So my first though upon getting home from uni was to open up server 2 and check if it had any slots for NVMe SSDs. Nope it does not. Ok not to worry, you can by adapters to let them work through PCIe x16 slots, which through my research seems to have a minimal or no impact to the read/write speeds. 

Now having verified we can, in fact, use NVMe SSDs, we need to look at our requirements:
1. We currently have two 1TB [Patriot P210 SSDs](https://www.hardware-corner.net/ssd-database/Patriot-P210/), so we need to replace those with two 1TB NVMe SSDs. 
2. They need to have DRAM (or DRAM cache)
3. And we need them to be affordable. 

Alright. Let's get looking, should be easy right! 

We'll start by filtering out SSDs that have no DRAM. To do this I went to [PC Part Picker](https://uk.pcpartpicker.com/list/) and filtered the storage list with NVMe set to yes, and set the cache range minimum to 512MB. For our affordability requirement I sorted this list by price (lowest to highest). 

![[Pasted image 20251215201354.png]]

So, let's go down the list:
- ~~Samsung 970 Evo Plus~~ - Sold Out 
- ~~Mushkin Vortex Redline~~ - Hadn't heard of manufacturer
- Samsung 980 Pro - Found for £150
- ~~Gigabyte AORUS Gen4 7300~~ - Sold Out
- ~~Western Digital WD_Black SN850X~~ - Earliest deliver too late 
- Samsung 990 Pro - Found for £112
- MSI SPATIUM M480 PRO - Found for £133
- ~~Crucial P5 Plus~~ - Sold Out

I looked at some more but it was more of the same - sold out or would deliver too late. So let's compare the three we've not ruled out above. Using [TechPowerup's SSD Database](https://www.techpowerup.com/ssd-specs/) I looked into the specs of these three for their 1TB sizes:

|                                                                                                                                     | Read (MB/s) | Write (MB/s) | DRAM Type      | DRAM Size (MB) | Endurance (TBW) | Price |
| ----------------------------------------------------------------------------------------------------------------------------------- | ----------- | ------------ | -------------- | -------------- | --------------- | ----- |
| [Samsung 980 Pro](https://www.techpowerup.com/ssd-specs/samsung-980-pro-1-tb.d47)                                                   | 7,000       | 5,000        | LPDDR4-1866    | 1,024          | 600             | £150  |
| [Samsung 990 Pro](https://www.techpowerup.com/ssd-specs/samsung-990-pro-1-tb.d861)                                                  | 7,450       | 6,900        | LPDDR4-1866    | 1,024          | 600             | £112  |
| [MSI SPATIUM M840 PRO](https://www.techpowerup.com/ssd-specs/msi-spatium-m480-pro-2-tb.d1514) (only 2TB size values were available) | 7,400       | 7,000        | DDR4-2666 CL19 | 2,048          | 1,400           | £133  |

So, let's immediately rule out the Samsung 980 Pro, it's worse than the other two and is more expensive. Now it's between the Samsung 990 Pro and the MSI SPATIUM M840 PRO. Since budget is an issue, I've opted for the Samsung 990 Pro as it has ever so slightly faster read, and only an ever so slightly lower write than the MSI SPATIUM, while being around £20 cheaper.

Awesome! After hours of searching we've found what we're going to buy! Let's find the nearest place that has it in stoc-- oh. Oh no. There's apparently only one left, not two 😐. Uhm. Ok, I need backup. Time to get my Dad, who certainly came through! He managed to not only find 2 Samsung 990 Pros that were in stock, but also managed to get himself a 20% discount, bringing them down to about £90 each! Thanks to Woodss and Naltam, we've got £97 in the server's account, so that's one paid for already, and my Dad covered the second. So they're on their way!

🚚 ☁

And they're here!