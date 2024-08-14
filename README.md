# sea-sandimport random

def generate_sand_pattern(width, height):
    sand_chars = ['.', ',', '`', '\'']  # Characters representing grains of sand
    pattern = ""

    for _ in range(height):
        line = "".join(random.choice(sand_chars) for _ in range(width))
        pattern += line + "\n"
    
    return pattern

# Parameters for the beach pattern
width = 40
height = 10

# Generate and display the sand pattern
sand_pattern = generate_sand_pattern(width, height)
print(sand_pattern)
