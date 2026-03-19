import React from "react";
import { StyleSheet, Text, View, FlatList, TouchableOpacity, SafeAreaView } from "react-native";

const data = [
    {
     id: '1', title:'Configurações'
    },
    {
     id: '2', title:'Perfil'
    },
    {
     id: '3', title:'Mensagens'
    },
    {
     id: '4', title:'Segurança'
    },
    {
     id: '5', title:'Ajuda'
    }
];

export default function App() {
    const renderItem = ({item}) => (
        <TouchableOpacity style={styles.button} onPress ={() => alert(`Você clicou em: ${item.title}`)}>
            <Text style={styles.buttonText}>{item.title}</Text>
        </TouchableOpacity>
    );


    return(
        <SafeAreaView style={styles.container}>
            <Text style={styles.header}> 
                Menu Principal 
            </Text>
            <FlatList data={data} renderItem={renderItem} keyExtraction={item => item.id} contentContainerStyle={styles.listPadding}/>
        </SafeAreaView>
    );
}

const styles = StyleSheet.create({
    container:{
        flex: 1,
        backgroundColor: '#f5f5f5'
    },
    header:{
        fontSize: 24,
        fontWeight: 'bold',
        textAlign: 'center',
        marginVertical: 20
    },
    listPadding:{
        paddingHorizontal: 20
    },
    button:{
        backgroundColor:'#007aff',
        padding: 15,
        borderRadius: 8,
        marginBottom: 10,
        alignItems: 'center',
        elevation: 2,
        shadowColor: '#000',
        shadowOffset:{ width: 0, height: 2},
        shadowOpacity: 0.1,
        shadowRadius: 4.5
    },
    buttonText:{
        color:'#fff',
        fontSize: 16,
        fontWeight: '600'
    }
});
