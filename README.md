import React from 'react';
import { StyleSheet, Text, View, Button } from 'react-native';

export default function App() {
  return (
    <View style={styles.container}>
      <Text style={styles.title}>Bienvenue à CovoiturageApp</Text>
      <Text style={styles.subtitle}>Choisissez une option</Text>
      <View style={styles.buttonContainer}>
        <Button title="Offrir un trajet" onPress={() => alert('Offrir un trajet')} />
        <Button title="Rechercher un trajet" onPress={() => alert('Rechercher un trajet')} />
      </View>
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    justifyContent: 'center',
    alignItems: 'center',
    backgroundColor: '#f5f5f5',
  },
  title: {
    fontSize: 24,
    fontWeight: 'bold',
    marginBottom: 20,
  },
  subtitle: {
    fontSize: 18,
    marginBottom: 40,
  },
  buttonContainer: {
    flexDirection: 'row',
    justifyContent: 'space-between',
    width: '80%',
  },
});
