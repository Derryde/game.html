def calculate_carbon_footprint(energy_consumption, transportation, waste_generation):
    # Define emission factors (values are placeholders and should be replaced with actual data)
    energy_emission_factor = 0.5  # kg CO2 per kWh
    transportation_emission_factor = 2.0  # kg CO2 per mile
    waste_emission_factor = 0.1  # kg CO2 per kg of waste

    # Calculate emissions for each category
    energy_emissions = energy_consumption * energy_emission_factor
    transportation_emissions = transportation * transportation_emission_factor
    waste_emissions = waste_generation * waste_emission_factor

    # Calculate total carbon footprint
    total_carbon_footprint = energy_emissions + transportation_emissions + waste_emissions

    return total_carbon_footprint

# Input data (replace these values with actual data)
energy_consumption = float(input("Enter energy consumption (kWh): "))
transportation = float(input("Enter transportation distance (miles): "))
waste_generation = float(input("Enter waste generation (kg): "))

# Calculate carbon footprint
carbon_footprint = calculate_carbon_footprint(energy_consumption, transportation, waste_generation)

# Display the result
print("\nTotal Carbon Footprint: {:.2f} kg CO2".format(carbon_footprint))

    
