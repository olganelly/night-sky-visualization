# night-sky-visualization
import matplotlib.pyplot as plt
import numpy as np

def generate_stars(num_stars=100):
    x = np.random.rand(num_stars) * 100  # Random x coordinates
    y = np.random.rand(num_stars) * 100  # Random y coordinates
    sizes = np.random.rand(num_stars) * 100  # Random star sizes
    return x, y, sizes

x, y, sizes = generate_stars()

plt.figure(figsize=(8, 8), facecolor='black')
plt.scatter(x, y, s=sizes, color='white', alpha=0.8)
plt.title("Night Sky with Stars", color='white')
plt.gca().set_facecolor('black')
plt.xticks([])
plt.yticks([])
plt.show()
hyu
