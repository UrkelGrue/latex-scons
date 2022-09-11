import os

# Initialize an internal construction environment
env = Environment(ENV = os.environ)

# Set construction variables for the pdflatex utility
env.Append(PDFLATEXFLAGS=['-halt-on-error', '--enable-write18'])

# Build the executable into the build folder
pdf = env.PDF('build/report.pdf', 'main.tex')

# Default target
Default(pdf)

# Remove build directory and contents
Clean(pdf, 'build')
