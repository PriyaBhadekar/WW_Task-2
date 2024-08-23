package com.example.entities;

import javax.persistence.Entity;
import javax.persistence.GeneratedValue;
import javax.persistence.GenerationType;
import javax.persistence.Id;
import javax.persistence.Column;
import javax.persistence.OneToMany;
import java.util.Set;

@Entity
public class FinancialAdvisor {
    
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long advisorId;

    @Column(nullable = false)
    private String name;

    @Column(nullable = false)
    private String contactInfo;

    @OneToMany(mappedBy = "financialAdvisor")
    private Set<Client> clients;

    // Default constructor
    public FinancialAdvisor() {
    }

    // Parameterized constructor
    public FinancialAdvisor(Long advisorId, String name, String contactInfo) {
        this.advisorId = advisorId;
        this.name = name;
        this.contactInfo = contactInfo;
    }

    // Getters and Setters
    public Long getAdvisorId() {
        return advisorId;
    }

    public void setAdvisorId(Long advisorId) {
        this.advisorId = advisorId;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getContactInfo() {
        return contactInfo;
    }

    public void setContactInfo(String contactInfo) {
        this.contactInfo = contactInfo;
    }

    public Set<Client> getClients() {
        return clients;
    }

    public void setClients(Set<Client> clients) {
        this.clients = clients;
    }
}
