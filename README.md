# How to Restore `PS1` in Your Terminal

If you have accidentally modified the `PS1` value or want to restore it to its default, follow the steps below. This guide will walk you through the process of restoration on Linux systems, including distributions like **Debian** and **Kali Linux**.

---

## What is `PS1`?

The `PS1` variable defines the format of your **terminal prompt**, which is the text that appears before you can enter commands. If you notice that your terminal prompt has changed or is showing incorrect information, the `PS1` value might have been altered.

---

# Solution: Restore `PS1`

### Step 1: Check the `.bashrc` File

The file that configures the terminal prompt is `.bashrc`, located in your home directory (`~`). To restore `PS1`, we need to edit this file.

## 2. Editing `.bashrc` with **`nano`** or **`vim`**

Now, you need to open the `.bashrc` file to restore the `PS1` value. Depending on your preference, you can use either **`nano`** or **`mousepad`**. Both are text editors available in most Linux distributions. Below are the instructions for each editor:

---

### Editing `.bashrc` with **`nano`**

**`nano`** is a simple, easy-to-use text editor. Here’s how to use it to edit your `.bashrc` file:

1. Open a terminal and type the following command:
   ```bash
   sudo nano ~/.bashrc
### Editing `.bashrc` with **`mousepad`**
This option is much easier because you don’t have to tab through the sections; you can go directly to it, and you can even search for it by pressing `Ctrl+F`, you will search "PS1" and you will gonna click the down arrow on the interface.

Once you have located the `PS1`, you will do the following:

1. **Uncomment the `PS1` line** by adding a `#` at the beginning of the line, which will disable the function from running.
   
2. Then, above the `PS1` line, add the following line to set your custom prompt:

   ```bash
   PS1='\n\[\e[38;5;43m\]┌──(\[\e[38;5;33;1m\]\u㉿\H:\[\e[0;38;5;43m\])-[\[\e[0;1m\]\w\[\e[0;38;5;43m\]]\n└─\[\e[38;5;33;1m\]\\$\[\e[0m\] '

   
