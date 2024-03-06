# Raptom
def calculate_sum_from_file(filename):
    total = 0
        with open(filename, 'r') as file:
                for line in file:
                            try:
                                            number = float(line.strip())
                                                            total += number
                                                                        except ValueError:
                                                                                        print(f"Warning: Skipped line '{line.strip()}' as it is not a valid number.")
                                                                                            return total

                                                                                            if __name__ == "__main__":
                                                                                                filename = input("Enter the name of the file containing the sequence of numbers: ")
                                                                                                    try:
                                                                                                            sum_result = calculate_sum_from_file(filename)
                                                                                                                    print(f"The sum of the numbers in '{filename}' is: {sum_result}")
                                                                                                                        except FileNotFoundError:
                                                                                                                                print(f"Error: File '{filename}' not found.")
                                                                                                                                