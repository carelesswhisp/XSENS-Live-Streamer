# XSENS-Live-Streamer
A tool to stream from Xsens MVN to unity3d with the basic free license 

---
🚨 **Warning:** This product is in **active development/beta**. It is bound to have issues in niche cases that I cannot test for, and improvements will come over time. **Updates are not guaranteed** on any specific schedule. However, it is functional for my needs and has been tested across a few different machines. **All known glitches are shown in the demo video on Itch.io.**  

👉 **Only purchase if you understand this**:  
🔗 **[Buy on Itch.io](https://moliminous.itch.io/xsens)**  

---

## Background

Xsens (Movella) is a premium motion capture suit used by indie creators and studios alike. Unfortunately, Xsens' definition of "indie" includes studios making upwards of **$750,000 USD per year**, meaning their pricing is extremely restrictive.  

Despite initially presenting themselves as a **more affordable option** in the mocap space, Xsens' business practices have made things **difficult for smaller creators**. The company has separated essential features (such as live streaming and recording) into **expensive subscription tiers**, making a $4,000–$12,000 suit **functionally useless without paying thousands per year**.  

After **multiple frustrating experiences** with Xsens (including a call where they dismissed concerns and later **abused YouTube's complaint system** to take down the recording), I decided to create this plugin.  

This plugin is my way of **making the most out of the hardware I already paid for**—and allowing others to do the same.  

---

## ❓ What Does This Plugin Do?

This plugin allows **Xsens MVN data to be streamed into Unity3D**.  

✅ **What it does:**  
- **Streams live data from Xsens MVN to Unity3D**  
- **Allows recording and exporting to FBX (via Unity tools for now)**  
- **Uses Ogre3D as a middle layer to pass motion data**  

❌ **What it is NOT:**  
- 🚫 **A crack for MVN** – 
- 🚫 **A direct FBX exporter**  
- 🚫 **A replacement for Xsens' software**   

---

## 🔴 Current Issues & Bugs  

- **Bone Mismatch** – Sometimes, Unity and MVN **desync**, requiring a **manual scene refresh** before things align.  
- **Hand Rotation Bug** – If you’re not using **Xsens-supported gloves** (e.g., **Manus**), your hands may default to pointing down. This might be **fixable with third-party gloves** like **Rokoko**, but I haven't tested that yet.  

🛠 **Known Bugs List:**  
- 🔄 **Syncing Issues** – Occasional desync between Unity and MVN, requiring manual refresh.  
- 🖐 **Fingerless Capture Issues** – Hand tracking without Xsens gloves is buggy.  

---

## 💰 Why Charge for This?  

1. Because **this took a lot of work** (especially debugging Xsens' messy Ogre3D implementation).  
2. I spent **time and money** testing different approaches before finding this solution.  
3. **Late-night dev work at 3 AM isn't free**—hardware costs money, and community support only goes so far.  
4. …Also, **the RTX 5090 is going to be $2,000**, so, like…  

**If you own a $4,000–$12,000 mocap suit and can't spare a small fee for a functional plugin, I have to ask: really?**  

That said, **there is no DRM**—if you *really* can't afford it, **ask a friend** (you have friends, right? …Right? )  

---

## 🔧 Installation Guide  

1️⃣ **Drop the plugin** into your `MVN plugin` folder.  
2️⃣ **Edit `ogre_plugin.cfg`** and add:  
   ```ini
   Plugin=BipedStreamerPlugin
   ```  
3️⃣ **Right-click** `mvn.exe` → **Properties**.  
4️⃣ Go to **Compatibility** → Enable **Run as Administrator**.  
5️⃣ **Install a crypto miner** (joking… unless? 👀)  
6️⃣ **Profit.**  

---

## 🔮 Future Plans  

- ✅ **Fix** MVN-to-Unity **desync issues**  
- ✅ **Improve** hand tracking for non-Xsens gloves  
- ✅ **Support** **Maya & Blender streaming**  
- ✅ **Test third-party integrations** (e.g., **Rokoko**)  

---

## 📢 Issues & Bug Reports  

⚠️ **Found a bug?** Report it here on GitHub under the **Issues** tab.  
📢 **Feature requests?** Open a **Discussion**.  

---

## 📌 Legal Note  

This project **does NOT modify or crack Xsens MVN software**. It is a standalone plugin that interacts with **Ogre3D**, an open-source rendering engine.  

🔗 **[Itch.io Store Page](https://moliminous.itch.io/xsens)**  


