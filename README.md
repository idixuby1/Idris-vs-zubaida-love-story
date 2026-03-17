import time

def show_text(text, delay=0.04):
    for char in text:
        print(char, end='', flush=True)
        time.sleep(delay)
    print("\n")

def wait():
    input("👉 Press Enter to continue...\n")

# TITLE
show_text("❤️ IDRIS ❤️ ZUBAIDA ❤️\n", 0.08)
wait()

# STORY PART 1
show_text("Idris first noticed Zubaida on a quiet Monday morning in school.")
show_text("The sun was just rising, casting a soft golden light across the field.")
show_text("Students were slowly gathering in groups.")
show_text("But something about her made him pause...")
wait()

# PART 2
show_text("Days passed... then weeks.")
show_text("Idris kept seeing her but never spoke.")
show_text("Deep inside, something was growing.")
show_text("Not just a crush... something deeper.")
wait()

# PART 3
show_text("One afternoon, everything changed.")
show_text("They were assigned to the same group.")
show_text("Idris was nervous... but excited.")
show_text("Zubaida smiled warmly at him.")
show_text("That moment gave him courage.")
wait()

# PART 4
show_text("They began talking more—about school, dreams, and life.")
show_text("Idris saw she was kind, intelligent, and full of ambition.")
show_text("Zubaida saw something special in Idris too.")
show_text("Their friendship grew stronger every day.")
wait()

# PART 5
show_text("But Idris was hiding something...")
show_text("His feelings were growing stronger.")
wait()

# CONFESSION
show_text("One evening, Idris finally spoke...")
show_text('"Zubaida... I think I’ve fallen in love with you."')
wait()

show_text("Silence filled the air...")
show_text('Then she smiled softly...')
show_text('"Idris... I feel the same way."')
wait()

# LOVE GROWS
show_text("From that moment, everything changed.")
show_text("They supported each other in everything.")
show_text("Their love grew stronger every day.")
wait()

# PROPOSAL
show_text("Years later, under a sky full of stars...")
show_text('"I don’t just want you now... I want you forever."')
show_text('"Will you marry me?"')
wait()

show_text('"Yes, Idris... I will." ❤️')
wait()

# ENDING
show_text("Their wedding was filled with joy and happiness.")
show_text("They became not just lovers, but life partners.")
show_text("And their love story became forever... ♾️")

print("\n❤️ THE END ❤️")
import tkinter as tk

# STORY PARTS
story = [
"❤️ IDRIS ❤️ ZUBAIDA ❤️",

"Idris first noticed Zubaida on a quiet Monday morning in school.\nThe sun was rising gently across the field...",

"Days passed... weeks passed...\nBut something inside him kept growing.",

"They were assigned to the same group.\nThat moment changed everything.",

"They talked more—about dreams, life, and school.\nTheir friendship became stronger.",

"But Idris was hiding something...\nHis feelings were growing.",

"One evening...\n'I think I’ve fallen in love with you,' Idris said.",

"Zubaida smiled softly...\n'I feel the same way.' ❤️",

"Their love grew stronger through time.\nThey supported each other always.",

"Years later under the stars...\n'Will you marry me?'",

"'Yes, Idris... I will.' 💍",

"Marriage came with challenges...\nBut their love never changed.",

"They became each other's peace.\nEach other's strength.",

"'Do you remember when we met?' Idris asked.",

"'You were my answered prayer,' Zubaida replied.",

"Their love story was not just a beginning...\nIt was forever. ♾️❤️"
]

# APP
index = 0

def next_part():
    global index
    if index < len(story) - 1:
        index += 1
        text_label.config(text=story[index])
    else:
        text_label.config(text="❤️ THE END ❤️")

# WINDOW
root = tk.Tk()
root.title("Idris ❤️ Zubaida Love Story")
root.geometry("400x400")
root.configure(bg="#1e1e2f")

# TEXT
text_label = tk.Label(
    root,
    text=story[0],
    wraplength=350,
    font=("Segoe UI", 12),
    fg="white",
    bg="#1e1e2f",
    justify="center"
)
text_label.pack(expand=True
